---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2b6b956dcca7ed3540972bae6ff2ba130baaae3f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144490"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="ebd7f-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebd7f-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="ebd7f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ebd7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebd7f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ebd7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebd7f-106">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="ebd7f-106">Contains properties for App configuration setting item.</span></span>

## <a name="properties"></a><span data-ttu-id="ebd7f-107">属性</span><span class="sxs-lookup"><span data-stu-id="ebd7f-107">Properties</span></span>
|<span data-ttu-id="ebd7f-108">属性</span><span class="sxs-lookup"><span data-stu-id="ebd7f-108">Property</span></span>|<span data-ttu-id="ebd7f-109">类型</span><span class="sxs-lookup"><span data-stu-id="ebd7f-109">Type</span></span>|<span data-ttu-id="ebd7f-110">说明</span><span class="sxs-lookup"><span data-stu-id="ebd7f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebd7f-111">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="ebd7f-111">appConfigKey</span></span>|<span data-ttu-id="ebd7f-112">字符串</span><span class="sxs-lookup"><span data-stu-id="ebd7f-112">String</span></span>|<span data-ttu-id="ebd7f-113">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="ebd7f-113">app configuration key.</span></span>|
|<span data-ttu-id="ebd7f-114">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="ebd7f-114">appConfigKeyType</span></span>|[<span data-ttu-id="ebd7f-115">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="ebd7f-115">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="ebd7f-116">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="ebd7f-116">app configuration key type.</span></span> <span data-ttu-id="ebd7f-117">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="ebd7f-117">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="ebd7f-118">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="ebd7f-118">appConfigKeyValue</span></span>|<span data-ttu-id="ebd7f-119">String</span><span class="sxs-lookup"><span data-stu-id="ebd7f-119">String</span></span>|<span data-ttu-id="ebd7f-120">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="ebd7f-120">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ebd7f-121">关系</span><span class="sxs-lookup"><span data-stu-id="ebd7f-121">Relationships</span></span>
<span data-ttu-id="ebd7f-122">无</span><span class="sxs-lookup"><span data-stu-id="ebd7f-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ebd7f-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebd7f-123">JSON Representation</span></span>
<span data-ttu-id="ebd7f-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebd7f-124">Here is a JSON representation of the resource.</span></span>
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




