---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d5016539583083b7604ec143797592f2218a6c4
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2020
ms.locfileid: "43086040"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerTaskDetails = {
  previewType: "noPreview",
  references: {
    http%3A//developer%2Emicrosoft%2Ecom:{
      @odata.type: "microsoft.graph.plannerExternalReference",
      alias: "Documentation",
      previewPriority: " !",
      type: "Other"
    },
    https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer:{
      @odata.type: "microsoft.graph.plannerExternalReference",
      previewPriority: "  !!",
    },
    http%3A//www%2Ebing%2Ecom: null
  },
  checklist: {
    95e27074-6c4a-447a-aa24-9d718a0b86fa:{
      @odata.type: "microsoft.graph.plannerChecklistItem",
      title: "Update task details",
      isChecked: true
    },
    d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff:{
      @odata.type: "microsoft.graph.plannerChecklistItem",
      isChecked: true,
    },
    a93c93c5-10a6-4167-9551-8bafa09967a7: null
  }
};

let res = await client.api('/planner/tasks/{task-id}/details')
    .update(plannerTaskDetails);

```