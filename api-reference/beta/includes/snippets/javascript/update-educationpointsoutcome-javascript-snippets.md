---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c1bd68c5719683712195fc00a5b08d6a8f603e93cd470af9e1853e348fd338e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218559"
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

await client.api('/education/classes/{id}/assignments/{id}/submissions/{id}/outcomes/{id}')
    .version('beta')
    .update(educationOutcome);

```