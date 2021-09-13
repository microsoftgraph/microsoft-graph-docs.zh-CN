---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5267d8ed0dfbd2b1078a78d9cf0318a4b684e640
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59095182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSubmission = {
};

await client.api('/education/classes/b07edbef-7420-4b3d-8f7c-d599cf21e069/assignments/222bd-b7d2-4d64-8a22-74b722ce2fc6/submissions/803fb5dd-3553-455f-3d94-f79fb54a1003/setUpResourcesFolder')
    .post(educationSubmission);

```