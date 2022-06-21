---
title: cloudPcProvisioningPolicy 资源类型
description: 表示云电脑预配策略。
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 5c9e851bf2a8723507e1eaa84bc014a715908770
ms.sourcegitcommit: da9079132db3261aed80e6fc4b9314d16e0847b3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/21/2022
ms.locfileid: "66186937"
---
# <a name="cloudpcprovisioningpolicy-resource-type"></a>cloudPcProvisioningPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示云电脑预配策略。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 provisioningPolicies](../api/virtualendpoint-list-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 集合|列出 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性和关系。|
|[获取 cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-get.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|读取 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性和关系。|
|[创建 cloudPcProvisioningPolicy](../api/virtualendpoint-post-provisioningpolicies.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|创建新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。|
|[更新 cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-update.md)|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|更新 [cloudPcProvisioningPolicy 对象的](../resources/cloudpcprovisioningpolicy.md) 属性。|
|[删除 cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-delete.md)|无|删除 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。|
|[分配 cloudPcProvisioningPolicy](../api/cloudpcprovisioningpolicy-assign.md)|无 |将 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 分配给用户组。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|alternateResourceUrl|String|链接到此预配策略的备用资源的 URL。 只读。|
|cloudPcGroupDisplayName|String|云电脑所在的云电脑组的显示名称。 只读。|
|说明|String|预配策略说明。|
|displayName|String|预配策略的显示名称。|
|domainJoinConfiguration|[cloudPcDomainJoinConfiguration](../resources/cloudpcdomainjoinconfiguration.md)|指定云电脑如何加入Azure Active Directory。|
|gracePeriodInHours|Int32|重新预配/取消预配前要等待的小时数。 只读。|
|id|String|云电脑预配策略的唯一标识符。 只读。|
|imageDisplayName|String|要预配的 OS 映像的显示名称。|
|imageId|String|要在云电脑上预配的 OS 映像的 ID。 库类型图像的格式为：{publisher_offer_sku}。 每个参数支持的值如下所示：<ul><li>发布者：Microsoftwindowsdesktop。</li> <li>offer： windows-ent-cpc.</li> <li>sku： 21h1-ent-cpc-m365， 21h1-ent-cpc-os、20h2-ent-cpc-m365、20h2-ent-cpc-os、20h1-ent-cpc-m365、20h1-ent-cpc-os、19h2-ent-cpc-m365 和 19h2-ent-cpc-os。</li></ul>|
|imageType|cloudPcProvisioningPolicyImageType|要在云电脑上预配) 自定义或库 (OS 映像的类型。 可取值为：`gallery`、`custom`。|
|localAdminEnabled|Boolean|指示是否启用本地管理员选项。 如果启用了本地管理员选项，则最终用户可以是云电脑设备的管理员。 只读。|
|managedBy|[cloudPcManagementService](../resources/cloudpconpremisesconnection.md#cloudpcmanagementservice-values)|指定管理 Azure 网络连接的服务。 可取值为：`windows365`、`devBox`、`unknownFutureValue`。 只读。|
|microsoftManagedDesktop|[microsoftManagedDesktop](../resources/microsoftManagedDesktop.md)|Microsoft 托管桌面的特定设置，使客户能够获得云电脑的托管设备体验。 在启用Microsoft 托管桌面之前，管理员必须对其进行配置。|
|onPremisesConnectionId|String|cloudPcOnPremisesConnection 的 ID。 若要确保云电脑具有网络连接且它们已加入域，请选择与云电脑服务验证的虚拟网络的连接。|
|windowsSettings|[cloudPcWindowsSettings](../resources/cloudpcwindowssettings.md)|为此预配策略创建云电脑时要配置的特定Windows设置。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|assignments|[cloudPcProvisioningPolicyAssignment](../resources/cloudpcprovisioningpolicyassignment.md) 集合|预配策略分配的定义集合。 表示已分配预配策略的 Azure AD 中的一组Microsoft 365组和安全组。 仅在 `$expand` 上返回。 请参阅获取分配关系的示 [例](../api/cloudpcprovisioningpolicy-get.md) 。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "alternateResourceUrl": "String",
  "cloudPcGroupDisplayName": "String",
  "description": "String",
  "displayName": "String",
  "domainJoinConfiguration": {
    "@odata.type": "microsoft.graph.cloudPcDomainJoinConfiguration"
  },
  "gracePeriodInHours": "Integer",
  "id": "String (identifier)",
  "imageDisplayName": "String",
  "imageId": "String",
  "imageType": "String",
  "localAdminEnabled": "Boolean",
  "managedBy": "String",
  "microsoftManagedDesktop": {
    "type": "String",
    "profile": "String"
  },
  "onPremisesConnectionId": "String",
  "windowsSettings": {
    "@odata.type": "microsoft.graph.cloudPcWindowsSettings"
  }
}
```
