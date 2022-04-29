---
title: subjectSet 复杂类型
description: 访问包分配策略的请求、审批和分配评审设置中使用的类型的抽象基类型。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0a266aea0693c6faf994da0fd829b8cacdee619e
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133116"
---
# <a name="subjectset-complex-type"></a>subjectSet 复杂类型

命名空间：microsoft.graph

在权利管理访问包分配策略和角色管理策略中使用的共享对象。

+ 在权利管理中，用于访问包分配策略的请求、批准和分配评审设置。
+ 在角色管理策略中，用于角色管理策略规则中定义的审批设置。

这是由以下派生类型继承的抽象基类型：
+ [singleUser](singleuser.md)
+ [singleServicePrincipal](singleserviceprincipal.md)
+ [groupMembers](groupmembers.md)
+ [connectedOrganizationMembers](connectedorganizationmembers.md)
+ [requestorManager](requestormanager.md)
+ [internalSponsors](internalsponsors.md)
+ [externalSponsors](externalsponsors.md)
+ [targetManager](targetmanager.md)
+ [targetApplicationOwners](targetapplicationowners.md)


## <a name="properties"></a>属性

无。
## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.subjectSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.subjectSet"
}
```


