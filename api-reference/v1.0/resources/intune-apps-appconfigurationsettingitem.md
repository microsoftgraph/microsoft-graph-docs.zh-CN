---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b7145b7adf9aed622af8ebb3a6a55c6456d7e8a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356301"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="52845-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="52845-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="52845-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="52845-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52845-105">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="52845-105">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="52845-106">属性</span><span class="sxs-lookup"><span data-stu-id="52845-106">Properties</span></span>
|<span data-ttu-id="52845-107">属性</span><span class="sxs-lookup"><span data-stu-id="52845-107">Property</span></span>|<span data-ttu-id="52845-108">类型</span><span class="sxs-lookup"><span data-stu-id="52845-108">Type</span></span>|<span data-ttu-id="52845-109">说明</span><span class="sxs-lookup"><span data-stu-id="52845-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52845-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="52845-110">appConfigKey</span></span>|<span data-ttu-id="52845-111">String</span><span class="sxs-lookup"><span data-stu-id="52845-111">String</span></span>|<span data-ttu-id="52845-112">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="52845-112">app configuration key.</span></span>|
|<span data-ttu-id="52845-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="52845-113">appConfigKeyType</span></span>|[<span data-ttu-id="52845-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="52845-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="52845-115">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="52845-115">app configuration key type.</span></span> <span data-ttu-id="52845-116">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="52845-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="52845-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="52845-117">appConfigKeyValue</span></span>|<span data-ttu-id="52845-118">String</span><span class="sxs-lookup"><span data-stu-id="52845-118">String</span></span>|<span data-ttu-id="52845-119">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="52845-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52845-120">关系</span><span class="sxs-lookup"><span data-stu-id="52845-120">Relationships</span></span>
<span data-ttu-id="52845-121">无</span><span class="sxs-lookup"><span data-stu-id="52845-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52845-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52845-122">JSON Representation</span></span>
<span data-ttu-id="52845-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52845-123">Here is a JSON representation of the resource.</span></span>
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




