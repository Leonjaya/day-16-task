# day-16-task
function processResult1() {
    return asyncOperation1();
}

function processResult2(result1) {
    return asyncOperation2(result1);
}

function processResult3(result2) {
    return asyncOperation3(result2);
}

async function handleOperations() {
    try {
        const result1 = await processResult1();
        const result2 = await processResult2(result1);
        const result3 = await processResult3(result2);
        // Do something with result3
    } catch (err) {
        handleError(err);
    }
}
