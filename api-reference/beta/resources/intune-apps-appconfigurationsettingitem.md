---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3e71ad9bddd6595f6057463aa01116727e368c46
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459132"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="5b737-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="5b737-103">appConfigurationSettingItem resource type</span></span>

<span data-ttu-id="5b737-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b737-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b737-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5b737-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b737-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b737-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b737-107">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="5b737-107">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="5b737-108">属性</span><span class="sxs-lookup"><span data-stu-id="5b737-108">Properties</span></span>
|<span data-ttu-id="5b737-109">属性</span><span class="sxs-lookup"><span data-stu-id="5b737-109">Property</span></span>|<span data-ttu-id="5b737-110">类型</span><span class="sxs-lookup"><span data-stu-id="5b737-110">Type</span></span>|<span data-ttu-id="5b737-111">说明</span><span class="sxs-lookup"><span data-stu-id="5b737-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b737-112">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="5b737-112">appConfigKey</span></span>|<span data-ttu-id="5b737-113">String</span><span class="sxs-lookup"><span data-stu-id="5b737-113">String</span></span>|<span data-ttu-id="5b737-114">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="5b737-114">app configuration key.</span></span>|
|<span data-ttu-id="5b737-115">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="5b737-115">appConfigKeyType</span></span>|[<span data-ttu-id="5b737-116">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="5b737-116">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="5b737-117">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="5b737-117">app configuration key type.</span></span> <span data-ttu-id="5b737-118">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="5b737-118">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="5b737-119">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="5b737-119">appConfigKeyValue</span></span>|<span data-ttu-id="5b737-120">String</span><span class="sxs-lookup"><span data-stu-id="5b737-120">String</span></span>|<span data-ttu-id="5b737-121">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="5b737-121">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b737-122">关系</span><span class="sxs-lookup"><span data-stu-id="5b737-122">Relationships</span></span>
<span data-ttu-id="5b737-123">无</span><span class="sxs-lookup"><span data-stu-id="5b737-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b737-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5b737-124">JSON Representation</span></span>
<span data-ttu-id="5b737-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b737-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



