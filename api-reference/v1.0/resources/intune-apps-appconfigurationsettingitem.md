---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 91ccefc06ba6a635b9b18e07465ea0332c48f022
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030175"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="80c1e-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="80c1e-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="80c1e-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80c1e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80c1e-105">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="80c1e-105">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="80c1e-106">属性</span><span class="sxs-lookup"><span data-stu-id="80c1e-106">Properties</span></span>
|<span data-ttu-id="80c1e-107">属性</span><span class="sxs-lookup"><span data-stu-id="80c1e-107">Property</span></span>|<span data-ttu-id="80c1e-108">类型</span><span class="sxs-lookup"><span data-stu-id="80c1e-108">Type</span></span>|<span data-ttu-id="80c1e-109">说明</span><span class="sxs-lookup"><span data-stu-id="80c1e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80c1e-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="80c1e-110">appConfigKey</span></span>|<span data-ttu-id="80c1e-111">String</span><span class="sxs-lookup"><span data-stu-id="80c1e-111">String</span></span>|<span data-ttu-id="80c1e-112">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="80c1e-112">app configuration key.</span></span>|
|<span data-ttu-id="80c1e-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="80c1e-113">appConfigKeyType</span></span>|[<span data-ttu-id="80c1e-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="80c1e-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="80c1e-115">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="80c1e-115">app configuration key type.</span></span> <span data-ttu-id="80c1e-116">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="80c1e-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="80c1e-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="80c1e-117">appConfigKeyValue</span></span>|<span data-ttu-id="80c1e-118">String</span><span class="sxs-lookup"><span data-stu-id="80c1e-118">String</span></span>|<span data-ttu-id="80c1e-119">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="80c1e-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80c1e-120">关系</span><span class="sxs-lookup"><span data-stu-id="80c1e-120">Relationships</span></span>
<span data-ttu-id="80c1e-121">无</span><span class="sxs-lookup"><span data-stu-id="80c1e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80c1e-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80c1e-122">JSON Representation</span></span>
<span data-ttu-id="80c1e-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80c1e-123">Here is a JSON representation of the resource.</span></span>
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



