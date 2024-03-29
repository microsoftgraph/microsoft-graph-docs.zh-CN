---
title: sideLoadingKey 资源类型
description: 若要为租户安装业务线应用，Windows 8 8.1 设备需要 SideLoadingKey 实体。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc902bb1a6b1549f13e718c37db41321e0e1cbd5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046720"
---
# <a name="sideloadingkey-resource-type"></a>sideLoadingKey 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

若要为租户安装业务线应用，Windows 8 8.1 设备需要 SideLoadingKey 实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 sideLoadingKeies](../api/intune-onboarding-sideloadingkey-list.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 集合|列出 [sideLoadingKey 对象的属性和](../resources/intune-onboarding-sideloadingkey.md) 关系。|
|[获取 sideLoadingKey](../api/intune-onboarding-sideloadingkey-get.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|读取 [sideLoadingKey 对象的属性和](../resources/intune-onboarding-sideloadingkey.md) 关系。|
|[创建 sideLoadingKey](../api/intune-onboarding-sideloadingkey-create.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|创建新的 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) 对象。|
|[删除 sideLoadingKey](../api/intune-onboarding-sideloadingkey-delete.md)|无|删除 [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)。|
|[更新 sideLoadingKey](../api/intune-onboarding-sideloadingkey-update.md)|[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)|更新 [sideLoadingKey 对象](../resources/intune-onboarding-sideloadingkey.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|旁加载密钥唯一 ID。|
|value|String|Side Loading Key Value， it is 5x5 value， seperated by hiphens.|
|displayName|String|向 ITPro 管理员显示的旁加载密钥名称。|
|说明|String|旁加载 向 ITPro 管理员显示的密钥说明。|
|totalActivation|Int32|向 ITPro 管理员显示的旁加载密钥总激活。|
|lastUpdatedDateTime|String|向 ITPro 管理员显示的"旁加载密钥上次更新日期"。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```



