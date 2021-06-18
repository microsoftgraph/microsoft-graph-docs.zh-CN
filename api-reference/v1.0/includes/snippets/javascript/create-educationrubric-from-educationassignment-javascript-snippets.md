---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f8ad2f28dd1a96f3fc60a727694026fe5c58cd4
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationRubric = {
  '@odata.id': 'https://graph.microsoft.com/v1.0/education/me/rubrics/ceb3863e-6912-4ea9-ac41-3c2bb7b6672d'
};

await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/rubric/$ref')
    .put(educationRubric);

```