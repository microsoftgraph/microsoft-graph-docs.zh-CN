---
title: 审批资源类型
description: 与 accessPackageAssignmentRequest 或 userConsentRequest 关联的审批对象。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e9c459563fa776427dfebcc6c6063b9bda1da846
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730387"
---
# <a name="approval-resource-type"></a>审批资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD中](entitlementmanagement-root.md)，与 关联的决策的审批对象 `accessPackageAssignmentRequest` 。 单个步骤请求可以有一个与它关联的步骤，审批者可以处理该步骤。 同样，多步骤请求可以有多个与之关联的步骤，审批者可以执行这些步骤。 但是，在多步骤审批中，将显示挂起的步骤和之前完成的步骤。

在 [userConsentRequests](../resources/userconsentrequest.md)中，与请求关联的决策的审批对象。

在 ["角色管理](../resources/rolemanagement.md)"中，批准或拒绝角色分配的决策。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
|[获取审批](../api/approval-get.md) | [审批](approval.md) | 检索 **审批对象的属性** 。 |


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|审批对象的标识符。  在权利管理中，它是访问包分配请求 [的标识符相同的标识符](accesspackageassignmentrequest.md)。|
|步骤|[approvalStep](../resources/approvalstep.md) 集合|用于表示与在 approvalStage 中配置的审批过程中的单步 [相关的决定](../resources/approvalstage.md)。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|stages|[approvalStage](../resources/approvalstage.md) 集合|用于访问包分配策略 的 **requestApprovalSettings** 属性中审批设置的 **approvalStages** [属性](accesspackageassignmentpolicy.md)。 指定每个阶段的主要、回退和升级审批者。|


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.approval",
  "baseType": "microsoft.graph.entity",
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.approval",
  "id": "String (identifier)",
  "steps": [{
        "@odata.type": "#microsoft.graph.approvalStep"
    }]
}
```
