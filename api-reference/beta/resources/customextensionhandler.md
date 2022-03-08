---
title: customExtensionHandler 资源类型
description: 定义何时执行自定义访问包工作流扩展。
author: currenmehta
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 59873faa46acb6f258ca6308da2b9d29e323bf65
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338218"
---
# <a name="customextensionhandler-resource-type"></a>customExtensionHandler 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义何时执行自定义访问 [包工作流扩展](customaccesspackageworkflowextension.md)。

继承自 [实体](entity.md)。

## <a name="methods"></a>方法
无。

> [!NOTE]
>
> 1. 若要读取策略上的 customExtensionHandler 对象，请追加 `?$expand=customExtensionHandlers` 到 [GET accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-get.md) 请求。 例如，`GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/4540a08f-8ab5-43f6-a923-015275799197?$expand=customExtensionHandlers`。 有关详细信息，请参阅 [示例 2：检索策略的自定义扩展处理程序](../api/accesspackageassignmentpolicy-get.md#example-2-retrieve-the-custom-extension-handlers-for-a-policy)。
>
> 2. 若要从策略 **中删除 customExtensionHandlers** 对象，请调用 [Update accessPackageAssignmentPolicy](../api/accesspackageassignmentpolicy-update.md) ，将 customExtensionHandlers 属性指定为空集合。 有关详细信息，请参阅示例 [2：从策略中删除 customExtensionHandlers](../api/accesspackageassignmentpolicy-update.md#example-2-remove-the-customextensionhandlers-from-a-policy)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String| 阶段的标识符。 继承自 [实体](../resources/entity.md)。|
|stage|accessPackageCustomExtensionStage|指示访问包自定义扩展运行时访问包分配请求工作流的阶段。 可取值包括：`assignmentRequestCreated`、`assignmentRequestApproved`、`assignmentRequestGranted`、`assignmentRequestRemoved`、`assignmentFourteenDaysBeforeExpiration`、`assignmentOneDayBeforeExpiration`、`unknownFutureValue`。 |

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|customExtension|[customAccessPackageWorkflowExtension](../resources/customaccesspackageworkflowextension.md)|指示将在此阶段执行哪个自定义工作流扩展。 可为 NULL。 支持 `$expand`。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.customExtensionHandler",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customExtensionHandler",
  "id": "String (identifier)",
  "stage": "String"
}
```

