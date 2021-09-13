---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 985ee9900dae178e4d0660b5eb3d9f91e841dc9eca58c5b832039a785d7f33f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103781"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerTaskDetails = {
  previewType: 'noPreview',
  references: {
    'http%3A//developer%2Emicrosoft%2Ecom':{
      '@odata.type': 'microsoft.graph.plannerExternalReference',
      alias: 'Documentation',
      previewPriority: ' !',
      type: 'Other'
    },
    'https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer':{
      '@odata.type': 'microsoft.graph.plannerExternalReference',
      previewPriority: '  !!',
    },
    'http%3A//www%2Ebing%2Ecom': null
  },
  checklist: {
    '95e27074-6c4a-447a-aa24-9d718a0b86fa':{
      '@odata.type': 'microsoft.graph.plannerChecklistItem',
      title: 'Update task details',
      isChecked: true
    },
    'd280ed1a-9f6b-4f9c-a962-fb4d00dc50ff':{
      '@odata.type': 'microsoft.graph.plannerChecklistItem',
      isChecked: true,
    },
    'a93c93c5-10a6-4167-9551-8bafa09967a7': null
  }
};

await client.api('/planner/tasks/{task-id}/details')
    .update(plannerTaskDetails);

```