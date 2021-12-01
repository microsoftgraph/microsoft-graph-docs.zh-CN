---
title: externalSponsors 复杂类型
description: 标识与租户中将允许其成为审批者的另一个用户的关系。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 34db10f8efe76d324d2b6577a0e7a5efcb311dc8
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242215"
---
# <a name="externalsponsors-complex-type"></a>externalSponsors 复杂类型

命名空间：microsoft.graph

在访问包分配策略的审批阶段使用。
它是 [subjectSet](subjectset.md)的子类型，其中值指示请求用户的已连接组织 `@odata.type` 外部发起 `#microsoft.graph.externalSponsors` 人将是审批者。 此审批者仅适用于来自已连接组织一部分的用户的请求。  使用 externalSponsors 创建访问包分配策略审批阶段时，还应包括另一个审批者，如单个用户或组的成员，以防连接的组织没有外部发起人。

## <a name="properties"></a>属性

无。
## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalSponsors",
  "baseType": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalSponsors"
}
```



