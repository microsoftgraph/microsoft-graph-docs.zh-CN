---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23e499e3b359575a20b81a1de598b2065d5bf96c
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignmentSettings = {
  submissionAnimationDisabled: true
};

await client.api('/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignmentSettings')
    .update(educationAssignmentSettings);

```