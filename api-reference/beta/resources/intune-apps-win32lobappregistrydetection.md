---
title: win32LobAppRegistryDetection 资源类型
description: 包含用于检测 Win32 应用程序的注册表属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0fbd54fe4ed8f7df35ae6acdcde8722b98d1c24a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335548"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="811e0-103">win32LobAppRegistryDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="811e0-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="811e0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="811e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="811e0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="811e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="811e0-106">包含用于检测 Win32 应用程序的注册表属性</span><span class="sxs-lookup"><span data-stu-id="811e0-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="811e0-107">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="811e0-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="811e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="811e0-108">Properties</span></span>
|<span data-ttu-id="811e0-109">属性</span><span class="sxs-lookup"><span data-stu-id="811e0-109">Property</span></span>|<span data-ttu-id="811e0-110">类型</span><span class="sxs-lookup"><span data-stu-id="811e0-110">Type</span></span>|<span data-ttu-id="811e0-111">说明</span><span class="sxs-lookup"><span data-stu-id="811e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="811e0-112">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="811e0-112">check32BitOn64System</span></span>|<span data-ttu-id="811e0-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="811e0-113">Boolean</span></span>|<span data-ttu-id="811e0-114">一个值, 该值指示此注册表路径是否用于检查64位系统上的32位应用</span><span class="sxs-lookup"><span data-stu-id="811e0-114">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="811e0-115">keyPath</span><span class="sxs-lookup"><span data-stu-id="811e0-115">keyPath</span></span>|<span data-ttu-id="811e0-116">String</span><span class="sxs-lookup"><span data-stu-id="811e0-116">String</span></span>|<span data-ttu-id="811e0-117">用于检测 Win32 业务线 (LoB) 应用程序的注册表项路径</span><span class="sxs-lookup"><span data-stu-id="811e0-117">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="811e0-118">等值</span><span class="sxs-lookup"><span data-stu-id="811e0-118">valueName</span></span>|<span data-ttu-id="811e0-119">String</span><span class="sxs-lookup"><span data-stu-id="811e0-119">String</span></span>|<span data-ttu-id="811e0-120">注册表值名称</span><span class="sxs-lookup"><span data-stu-id="811e0-120">The registry value name</span></span>|
|<span data-ttu-id="811e0-121">detectionType</span><span class="sxs-lookup"><span data-stu-id="811e0-121">detectionType</span></span>|[<span data-ttu-id="811e0-122">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="811e0-122">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="811e0-123">注册表数据检测类型。</span><span class="sxs-lookup"><span data-stu-id="811e0-123">The registry data detection type.</span></span> <span data-ttu-id="811e0-124">可取值为：`notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="811e0-124">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="811e0-125">operator</span><span class="sxs-lookup"><span data-stu-id="811e0-125">operator</span></span>|[<span data-ttu-id="811e0-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="811e0-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="811e0-127">用于注册表数据检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="811e0-127">The operator for registry data detection.</span></span> <span data-ttu-id="811e0-128">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="811e0-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="811e0-129">detectionValue</span><span class="sxs-lookup"><span data-stu-id="811e0-129">detectionValue</span></span>|<span data-ttu-id="811e0-130">String</span><span class="sxs-lookup"><span data-stu-id="811e0-130">String</span></span>|<span data-ttu-id="811e0-131">注册表检测值</span><span class="sxs-lookup"><span data-stu-id="811e0-131">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="811e0-132">关系</span><span class="sxs-lookup"><span data-stu-id="811e0-132">Relationships</span></span>
<span data-ttu-id="811e0-133">无</span><span class="sxs-lookup"><span data-stu-id="811e0-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="811e0-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="811e0-134">JSON Representation</span></span>
<span data-ttu-id="811e0-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="811e0-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryDetection",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```



