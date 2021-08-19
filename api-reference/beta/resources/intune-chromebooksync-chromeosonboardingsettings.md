---
title: chromeOSOnboardingSettings 资源类型
description: 表示 Chromebook 租户设置的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 53b42eae58cbd68f4663290cd5d565e8fdf44c27bab676835054dcbc919a8935
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206786"
---
# <a name="chromeosonboardingsettings-resource-type"></a>chromeOSOnboardingSettings 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 Chromebook 租户设置的实体

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 chromeOSOnboardingSettingses](../api/intune-chromebooksync-chromeosonboardingsettings-list.md)|[chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 集合|列出 [chromeOSOnboardingSettings 对象的属性和](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 关系。|
|[获取 chromeOSOnboardingSettings](../api/intune-chromebooksync-chromeosonboardingsettings-get.md)|[chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|读取 [chromeOSOnboardingSettings 对象的属性和](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 关系。|
|[创建 chromeOSOnboardingSettings](../api/intune-chromebooksync-chromeosonboardingsettings-create.md)|[chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|创建新的 [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 对象。|
|[删除 chromeOSOnboardingSettings](../api/intune-chromebooksync-chromeosonboardingsettings-delete.md)|无|删除 [chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)。|
|[更新 chromeOSOnboardingSettings](../api/intune-chromebooksync-chromeosonboardingsettings-update.md)|[chromeOSOnboardingSettings](../resources/intune-chromebooksync-chromeosonboardingsettings.md)|更新 [chromeOSOnboardingSettings 对象](../resources/intune-chromebooksync-chromeosonboardingsettings.md) 的属性。|
|[connect 操作](../api/intune-chromebooksync-chromeosonboardingsettings-connect.md)|[chromeOSOnboardingStatus](../resources/intune-chromebooksync-chromeosonboardingstatus.md)|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|ChromebookTenant 的 ID|
|ownerUserPrincipalName|String|ChromebookTenant 的 OwnerUserPrincipalName|
|onboardingStatus|[onboardingStatus](../resources/intune-chromebooksync-onboardingstatus.md)|ChromebookTenant 的 OnboardingStatus。 可取值为：`unknown`、`inprogress`、`onboarded`、`failed`。|
|lastModifiedDateTime|DateTimeOffset|ChromebookTenant 的 LastModifiedDateTime|
|lastDirectorySyncDateTime|DateTimeOffset|ChromebookTenant 的 LastDirectorySyncDateTime|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chromeOSOnboardingSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chromeOSOnboardingSettings",
  "id": "String (identifier)",
  "ownerUserPrincipalName": "String",
  "onboardingStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "lastDirectorySyncDateTime": "String (timestamp)"
}
```




