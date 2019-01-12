---
title: win32LobAppRegistryDetection 资源类型
description: 包含要检测 Win32 应用程序的注册表属性
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 23362d7613d198bdd848205cbf20944e9a592f04
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923899"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="c6383-103">win32LobAppRegistryDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6383-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="c6383-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c6383-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6383-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c6383-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6383-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c6383-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6383-107">包含要检测 Win32 应用程序的注册表属性</span><span class="sxs-lookup"><span data-stu-id="c6383-107">Contains registry properties to detect a Win32 App</span></span>

<span data-ttu-id="c6383-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="c6383-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c6383-109">属性</span><span class="sxs-lookup"><span data-stu-id="c6383-109">Properties</span></span>
|<span data-ttu-id="c6383-110">属性</span><span class="sxs-lookup"><span data-stu-id="c6383-110">Property</span></span>|<span data-ttu-id="c6383-111">类型</span><span class="sxs-lookup"><span data-stu-id="c6383-111">Type</span></span>|<span data-ttu-id="c6383-112">Description</span><span class="sxs-lookup"><span data-stu-id="c6383-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6383-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="c6383-113">check32BitOn64System</span></span>|<span data-ttu-id="c6383-114">布尔</span><span class="sxs-lookup"><span data-stu-id="c6383-114">Boolean</span></span>|<span data-ttu-id="c6383-115">一个值，该值此注册表路径是否检查 64 位系统上的 32 位应用程序</span><span class="sxs-lookup"><span data-stu-id="c6383-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="c6383-116">keyPath</span><span class="sxs-lookup"><span data-stu-id="c6383-116">keyPath</span></span>|<span data-ttu-id="c6383-117">字符串</span><span class="sxs-lookup"><span data-stu-id="c6383-117">String</span></span>|<span data-ttu-id="c6383-118">注册表项路径来检测 Win32 业务线 (LoB) 应用程序</span><span class="sxs-lookup"><span data-stu-id="c6383-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="c6383-119">数值名称</span><span class="sxs-lookup"><span data-stu-id="c6383-119">valueName</span></span>|<span data-ttu-id="c6383-120">字符串</span><span class="sxs-lookup"><span data-stu-id="c6383-120">String</span></span>|<span data-ttu-id="c6383-121">注册表值名称</span><span class="sxs-lookup"><span data-stu-id="c6383-121">The registry value name</span></span>|
|<span data-ttu-id="c6383-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="c6383-122">detectionType</span></span>|[<span data-ttu-id="c6383-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="c6383-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="c6383-124">注册表数据检测类型。</span><span class="sxs-lookup"><span data-stu-id="c6383-124">The registry data detection type.</span></span> <span data-ttu-id="c6383-125">可取值为：`notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="c6383-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="c6383-126">operator</span><span class="sxs-lookup"><span data-stu-id="c6383-126">operator</span></span>|[<span data-ttu-id="c6383-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="c6383-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="c6383-128">注册表数据检测运算符。</span><span class="sxs-lookup"><span data-stu-id="c6383-128">The operator for registry data detection.</span></span> <span data-ttu-id="c6383-129">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="c6383-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="c6383-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="c6383-130">detectionValue</span></span>|<span data-ttu-id="c6383-131">字符串</span><span class="sxs-lookup"><span data-stu-id="c6383-131">String</span></span>|<span data-ttu-id="c6383-132">注册表检测值</span><span class="sxs-lookup"><span data-stu-id="c6383-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6383-133">Relationships</span><span class="sxs-lookup"><span data-stu-id="c6383-133">Relationships</span></span>
<span data-ttu-id="c6383-134">无</span><span class="sxs-lookup"><span data-stu-id="c6383-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6383-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6383-135">JSON Representation</span></span>
<span data-ttu-id="c6383-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6383-136">Here is a JSON representation of the resource.</span></span>
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





