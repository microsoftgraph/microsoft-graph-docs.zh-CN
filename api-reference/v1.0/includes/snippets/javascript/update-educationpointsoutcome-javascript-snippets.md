---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64aaafae6948ffbd3e20232bd4b3a280949893ba
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationOutcome = {
    '@odata.type':'#microsoft.graph.educationPointsOutcome',
    points: {
        '@odata.type':'#microsoft.graph.educationAssignmentPointsGrade',
        points: 85.0
    }
};

await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/outcomes/9c0f2850-ff8f-4fd6-b3ac-e23077b59141')
    .update(educationOutcome);

```