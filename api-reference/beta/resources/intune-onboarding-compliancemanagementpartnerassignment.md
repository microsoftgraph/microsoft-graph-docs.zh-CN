---
title: complianceManagementPartnerAssignment 资源类型
description: 针对合规性管理合作伙伴的用户组目标
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 51dc2a8f4861f160db6a3775526ec7fdd4e85ea7
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088215"
---
# <a name="compliancemanagementpartnerassignment-resource-type"></a>complianceManagementPartnerAssignment 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

针对合规性管理合作伙伴的用户组目标

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|组分配目标。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.complianceManagementPartnerAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.complianceManagementPartnerAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



