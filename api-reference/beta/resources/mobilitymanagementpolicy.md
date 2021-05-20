---
title: mobilityManagementPolicy 资源类型
description: 移动管理策略表示在 Azure AD 中配置的移动性管理应用程序的自动注册策略。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7f0c073d0737c634872009fffa5425ffe74f4e54
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547403"
---
# <a name="mobilitymanagementpolicy-resource-type"></a>mobilityManagementPolicy 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD 中，移动管理策略表示 MDM 或 MAM (移动管理自动注册) 配置。 这些策略仅适用于基于 Windows 10 操作系统及其派生 (Surface Hub、Hololens 等) 。 [自动注册](https://docs.microsoft.com/windows/client-management/mdm/azure-ad-and-microsoft-intune-automatic-mdm-enrollment-in-the-new-portal)使组织能够自动将设备注册到所选移动管理应用程序中，作为[Azure AD](https://docs.microsoft.com/azure/active-directory/devices/concept-azure-ad-join)加入或[Azure AD](https://docs.microsoft.com/azure/active-directory/devices/concept-azure-ad-register)注册过程的一部分，Windows 10注册。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 mobileDeviceManagementPolicies](../api/mobiledevicemanagementpolicies-list.md)|[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 集合|获取移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象及其属性的列表。|
|[获取 mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-get.md)|[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md)|读取移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性和关系。|
|[更新 mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-update.md)|无|更新移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性。|
|[列出 mobileDeviceManagementPolicy 的 includedGroups](../api/mobiledevicemanagementpolicies-list-includedgroups.md)|[group](../resources/group.md) 集合|列出移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的组。|
|[将组添加到 mobileDeviceManagementPolicy](../api/mobiledevicemanagementpolicies-post-includedgroups.md)|无|将组添加到移动设备管理 [应用程序的 mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象。|
|[从 mobileDeviceManagementPolicy 中删除组](../api/mobiledevicemanagementpolicies-delete-includedgroups.md)|无|从移动设备管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象中删除组。|
|[列出 mobileAppManagementPolicies](../api/mobileappmanagementpolicies-list.md)|[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 集合|获取移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象及其属性的列表。|
|[获取 mobileAppManagementPolicy](../api/mobileappmanagementpolicies-get.md)|[mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md)|读取移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性和关系。|
|[更新 mobileAppManagementPolicy](../api/mobileappmanagementpolicies-update.md)|无|更新移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的属性。|
|[列出 mobileAppManagementPolicy 的 includedGroups](../api/mobileappmanagementpolicies-list-includedgroups.md)|[group](../resources/group.md) 集合|列出移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象的组。|
|[将组添加到 mobileAppManagementPolicy](../api/mobileappmanagementpolicies-post-includedgroups.md)|无|将组添加到 [移动应用管理应用程序的 mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象。
|[从 mobileAppManagementPolicy 中删除组](../api/mobileappmanagementpolicies-delete-includedgroups.md)|无|从移动应用管理应用程序的 [mobilityManagementPolicy](../resources/mobilitymanagementpolicy.md) 对象中删除组。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|appliesTo|policyScope|指示移动管理策略的用户作用域。 可取值为：`none`、`all`、`selected`。|
|complianceUrl|String|移动管理应用程序的合规性 URL。|
|说明|String|移动管理应用程序的说明。|
|discoveryUrl|String|移动管理应用程序的发现 URL。|
|displayName|String|移动管理应用程序的显示名称。|
|id|String|移动管理应用程序的对象 ID。|
|termsOfUseUrl|String|移动管理应用程序的使用条款 URL。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|includedGroups|[group](../resources/group.md) 集合|移动性管理应用程序作用域下的 Azure AD 组（如果 appliesTo 为 ） `selected`|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobilityManagementPolicy",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "appliesTo": "String",
  "complianceUrl": "String",
  "description": "String",
  "discoveryUrl": "String",
  "displayName": "String",
  "termsOfUseUrl": "String"
}
```

<!-- uuid: 5c98f801-d1c4-44eb-ac11-f72b6754deda
2020-03-23T22:34:45.203Z -->
<!-- {
  "type": "#page.annotation",
  "description": "mobilityManagementPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
