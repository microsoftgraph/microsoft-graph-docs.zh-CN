---
title: win32LobAppRegistryDetection 资源类型
description: 包含用于检测 Win32 应用程序的注册表属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da9f63d4a16df728320e0f3144bee32ad90f2922
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490460"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="eb580-103">win32LobAppRegistryDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb580-103">win32LobAppRegistryDetection resource type</span></span>

<span data-ttu-id="eb580-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="eb580-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eb580-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eb580-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb580-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eb580-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb580-107">包含用于检测 Win32 应用程序的注册表属性</span><span class="sxs-lookup"><span data-stu-id="eb580-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="eb580-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="eb580-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb580-109">属性</span><span class="sxs-lookup"><span data-stu-id="eb580-109">Properties</span></span>
|<span data-ttu-id="eb580-110">属性</span><span class="sxs-lookup"><span data-stu-id="eb580-110">Property</span></span>|<span data-ttu-id="eb580-111">类型</span><span class="sxs-lookup"><span data-stu-id="eb580-111">Type</span></span>|<span data-ttu-id="eb580-112">说明</span><span class="sxs-lookup"><span data-stu-id="eb580-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb580-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="eb580-113">check32BitOn64System</span></span>|<span data-ttu-id="eb580-114">布尔</span><span class="sxs-lookup"><span data-stu-id="eb580-114">Boolean</span></span>|<span data-ttu-id="eb580-115">一个值，该值指示此注册表路径是否用于检查64位系统上的32位应用</span><span class="sxs-lookup"><span data-stu-id="eb580-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="eb580-116">keyPath</span><span class="sxs-lookup"><span data-stu-id="eb580-116">keyPath</span></span>|<span data-ttu-id="eb580-117">String</span><span class="sxs-lookup"><span data-stu-id="eb580-117">String</span></span>|<span data-ttu-id="eb580-118">用于检测 Win32 业务线（LoB）应用程序的注册表项路径</span><span class="sxs-lookup"><span data-stu-id="eb580-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="eb580-119">等值</span><span class="sxs-lookup"><span data-stu-id="eb580-119">valueName</span></span>|<span data-ttu-id="eb580-120">String</span><span class="sxs-lookup"><span data-stu-id="eb580-120">String</span></span>|<span data-ttu-id="eb580-121">注册表值名称</span><span class="sxs-lookup"><span data-stu-id="eb580-121">The registry value name</span></span>|
|<span data-ttu-id="eb580-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="eb580-122">detectionType</span></span>|[<span data-ttu-id="eb580-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="eb580-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="eb580-124">注册表数据检测类型。</span><span class="sxs-lookup"><span data-stu-id="eb580-124">The registry data detection type.</span></span> <span data-ttu-id="eb580-125">可取值为：`notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="eb580-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="eb580-126">operator</span><span class="sxs-lookup"><span data-stu-id="eb580-126">operator</span></span>|[<span data-ttu-id="eb580-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="eb580-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="eb580-128">用于注册表数据检测的运算符。</span><span class="sxs-lookup"><span data-stu-id="eb580-128">The operator for registry data detection.</span></span> <span data-ttu-id="eb580-129">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="eb580-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="eb580-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="eb580-130">detectionValue</span></span>|<span data-ttu-id="eb580-131">String</span><span class="sxs-lookup"><span data-stu-id="eb580-131">String</span></span>|<span data-ttu-id="eb580-132">注册表检测值</span><span class="sxs-lookup"><span data-stu-id="eb580-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb580-133">关系</span><span class="sxs-lookup"><span data-stu-id="eb580-133">Relationships</span></span>
<span data-ttu-id="eb580-134">无</span><span class="sxs-lookup"><span data-stu-id="eb580-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb580-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb580-135">JSON Representation</span></span>
<span data-ttu-id="eb580-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb580-136">Here is a JSON representation of the resource.</span></span>
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



