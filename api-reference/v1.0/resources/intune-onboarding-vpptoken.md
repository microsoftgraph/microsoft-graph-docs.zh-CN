---
title: vppToken 资源类型
description: 通过 Apple Volume Purchase Program 企业版或教育版为 iOS 应用购买多个许可证。 这涉及从 Apple 网站设置 Apple VPP 帐户并将 Apple VPP 企业版 或教育版令牌上传到 Intune。 然后可以将批量采购信息与 Intune 同步，并跟踪批量采购应用的使用情况。 可上传多个 Apple VPP 企业版或教育版令牌。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fd3d625969713c639661562fca517be3f9378b8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755705"
---
# <a name="vpptoken-resource-type"></a>vppToken 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

通过 Apple Volume Purchase Program 企业版或教育版为 iOS 应用购买多个许可证。 这涉及从 Apple 网站设置 Apple VPP 帐户并将 Apple VPP 企业版 或教育版令牌上传到 Intune。 然后可以将批量采购信息与 Intune 同步，并跟踪批量采购应用的使用情况。 可上传多个 Apple VPP 企业版或教育版令牌。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 vppTokens](../api/intune-onboarding-vpptoken-list.md)|[vppToken](../resources/intune-onboarding-vpptoken.md) 集合|列出 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。|
|[获取 vppToken](../api/intune-onboarding-vpptoken-get.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|读取 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性和关系。|
|[创建 vppToken](../api/intune-onboarding-vpptoken-create.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|创建新的 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象。|
|[删除 vppToken](../api/intune-onboarding-vpptoken-delete.md)|无|删除 [vppToken](../resources/intune-onboarding-vpptoken.md)。|
|[更新 vppToken](../api/intune-onboarding-vpptoken-update.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|更新 [vppToken](../resources/intune-onboarding-vpptoken.md) 对象的属性。|
|[syncLicenses 操作](../api/intune-onboarding-vpptoken-synclicenses.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|同步与特定 appleVolumePurchaseProgramToken 关联的许可证|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|这是创建 appleVolumePurchaseProgramToken 时自动生成的。 它是实体的键。|
|organizationName|String|与 Apple Volume Purchase Program 令牌关联的组织|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|与给定的 Apple Volume Purchase Program 令牌关联的批量购买计划的类型。 可取值为：`business`、`education`。 可取值为：`business`、`education`。|
|appleId|String|与给定的 Apple Volume Purchase Program 令牌关联的 Apple ID。|
|expirationDateTime|DateTimeOffset|Apple Volume Purchase Program 令牌的到期日期时间。|
|lastSyncDateTime|DateTimeOffset|上次利用 Apple Volume Purchase Program 服务并使用 Apple Volume Purchase Program 令牌完成应用程序同步的时间。|
|token|String|从 Apple Volume Purchase Program 下载的 Apple Volume Purchase Program 令牌字符串。|
|lastModifiedDateTime|DateTimeOffset|与 Apple Volume Purchase Program 令牌关联的上次修改日期时间。|
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Apple Volume Purchase Program 令牌的当前状态。 可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。 可取值为：`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM`。|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|使用 Apple Volume Purchase Program 令牌触发的上一次应用程序同步的当前同步状态。 可取值为：`none`、`inProgress`、`completed`、`failed`。 可取值为：`none`、`inProgress`、`completed`、`failed`。|
|automaticallyUpdateApps|Boolean|是否自动更新适用于 VPP 令牌的应用。|
|countryOrRegion|String|是否自动更新适用于 VPP 令牌的应用。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppToken"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "String (identifier)",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String"
}
```




