---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9806758caf1b3fafe6cbbc5be0a4573bdec5f6536535c4c71adc91772e054c61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163438"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addToReviewSet = {
    sourceCollection: {
        id: '1a9b4145d8f84e39bc45a7f68c5c5119'
    },
    additionalData: 'linkedFiles'
};

await client.api('/compliance/ediscovery/cases/080e8cad-f21f-4452-8826-0ddf7e949fdd/reviewSets/6fe25d32-8167-4625-b75c-c4181ccbd9d5/addToReviewSet')
    .version('beta')
    .post(addToReviewSet);

```