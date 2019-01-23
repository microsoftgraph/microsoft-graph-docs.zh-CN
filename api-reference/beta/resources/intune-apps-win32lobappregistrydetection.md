---
title: win32LobAppRegistryDetection 资源类型
description: 包含要检测 Win32 应用程序的注册表属性
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb10a96a14d3c26503b33191fbb3c1b883245da7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402662"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="d4dd3-103">win32LobAppRegistryDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4dd3-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="d4dd3-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d4dd3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4dd3-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d4dd3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4dd3-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4dd3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4dd3-107">包含要检测 Win32 应用程序的注册表属性</span><span class="sxs-lookup"><span data-stu-id="d4dd3-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="d4dd3-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="d4dd3-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d4dd3-109">属性</span><span class="sxs-lookup"><span data-stu-id="d4dd3-109">Properties</span></span>
|<span data-ttu-id="d4dd3-110">属性</span><span class="sxs-lookup"><span data-stu-id="d4dd3-110">Property</span></span>|<span data-ttu-id="d4dd3-111">类型</span><span class="sxs-lookup"><span data-stu-id="d4dd3-111">Type</span></span>|<span data-ttu-id="d4dd3-112">说明</span><span class="sxs-lookup"><span data-stu-id="d4dd3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4dd3-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="d4dd3-113">check32BitOn64System</span></span>|<span data-ttu-id="d4dd3-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4dd3-114">Boolean</span></span>|<span data-ttu-id="d4dd3-115">一个值，该值此注册表路径是否检查 64 位系统上的 32 位应用程序</span><span class="sxs-lookup"><span data-stu-id="d4dd3-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="d4dd3-116">keyPath</span><span class="sxs-lookup"><span data-stu-id="d4dd3-116">keyPath</span></span>|<span data-ttu-id="d4dd3-117">String</span><span class="sxs-lookup"><span data-stu-id="d4dd3-117">String</span></span>|<span data-ttu-id="d4dd3-118">注册表项路径来检测 Win32 业务线 (LoB) 应用程序</span><span class="sxs-lookup"><span data-stu-id="d4dd3-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="d4dd3-119">数值名称</span><span class="sxs-lookup"><span data-stu-id="d4dd3-119">valueName</span></span>|<span data-ttu-id="d4dd3-120">String</span><span class="sxs-lookup"><span data-stu-id="d4dd3-120">String</span></span>|<span data-ttu-id="d4dd3-121">注册表值名称</span><span class="sxs-lookup"><span data-stu-id="d4dd3-121">The registry value name</span></span>|
|<span data-ttu-id="d4dd3-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="d4dd3-122">detectionType</span></span>|[<span data-ttu-id="d4dd3-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="d4dd3-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="d4dd3-124">注册表数据检测类型。</span><span class="sxs-lookup"><span data-stu-id="d4dd3-124">The registry data detection type.</span></span> <span data-ttu-id="d4dd3-125">可取值为：`notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="d4dd3-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="d4dd3-126">operator</span><span class="sxs-lookup"><span data-stu-id="d4dd3-126">operator</span></span>|[<span data-ttu-id="d4dd3-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="d4dd3-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="d4dd3-128">注册表数据检测运算符。</span><span class="sxs-lookup"><span data-stu-id="d4dd3-128">The operator for registry data detection.</span></span> <span data-ttu-id="d4dd3-129">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="d4dd3-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="d4dd3-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="d4dd3-130">detectionValue</span></span>|<span data-ttu-id="d4dd3-131">String</span><span class="sxs-lookup"><span data-stu-id="d4dd3-131">String</span></span>|<span data-ttu-id="d4dd3-132">注册表检测值</span><span class="sxs-lookup"><span data-stu-id="d4dd3-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4dd3-133">关系</span><span class="sxs-lookup"><span data-stu-id="d4dd3-133">Relationships</span></span>
<span data-ttu-id="d4dd3-134">无</span><span class="sxs-lookup"><span data-stu-id="d4dd3-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4dd3-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4dd3-135">JSON Representation</span></span>
<span data-ttu-id="d4dd3-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4dd3-136">Here is a JSON representation of the resource.</span></span>
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




