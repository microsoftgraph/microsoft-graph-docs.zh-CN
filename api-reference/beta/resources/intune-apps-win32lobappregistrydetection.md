---
title: win32LobAppRegistryDetection 资源类型
description: 包含要检测 Win32 应用程序的注册表属性
ms.openlocfilehash: d0cab24f2f0eb4d0ad82d60285a4d0aca9ea6dda
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042531"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="2c58f-103">win32LobAppRegistryDetection 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c58f-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="2c58f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2c58f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c58f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2c58f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c58f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2c58f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c58f-107">包含要检测 Win32 应用程序的注册表属性</span><span class="sxs-lookup"><span data-stu-id="2c58f-107">Contains registry properties to detect a Win32 App</span></span>

<span data-ttu-id="2c58f-108">继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="2c58f-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2c58f-109">属性</span><span class="sxs-lookup"><span data-stu-id="2c58f-109">Properties</span></span>
|<span data-ttu-id="2c58f-110">属性</span><span class="sxs-lookup"><span data-stu-id="2c58f-110">Property</span></span>|<span data-ttu-id="2c58f-111">类型</span><span class="sxs-lookup"><span data-stu-id="2c58f-111">Type</span></span>|<span data-ttu-id="2c58f-112">说明</span><span class="sxs-lookup"><span data-stu-id="2c58f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c58f-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="2c58f-113">check32BitOn64System</span></span>|<span data-ttu-id="2c58f-114">布尔</span><span class="sxs-lookup"><span data-stu-id="2c58f-114">Boolean</span></span>|<span data-ttu-id="2c58f-115">一个值，该值此注册表路径是否检查 64 位系统上的 32 位应用程序</span><span class="sxs-lookup"><span data-stu-id="2c58f-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="2c58f-116">keyPath</span><span class="sxs-lookup"><span data-stu-id="2c58f-116">keyPath</span></span>|<span data-ttu-id="2c58f-117">字符串</span><span class="sxs-lookup"><span data-stu-id="2c58f-117">String</span></span>|<span data-ttu-id="2c58f-118">注册表项路径来检测 Win32 业务线 (LoB) 应用程序</span><span class="sxs-lookup"><span data-stu-id="2c58f-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="2c58f-119">数值名称</span><span class="sxs-lookup"><span data-stu-id="2c58f-119">valueName</span></span>|<span data-ttu-id="2c58f-120">字符串</span><span class="sxs-lookup"><span data-stu-id="2c58f-120">String</span></span>|<span data-ttu-id="2c58f-121">注册表值名称</span><span class="sxs-lookup"><span data-stu-id="2c58f-121">The registry value name</span></span>|
|<span data-ttu-id="2c58f-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="2c58f-122">detectionType</span></span>|[<span data-ttu-id="2c58f-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="2c58f-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="2c58f-124">注册表数据检测类型。</span><span class="sxs-lookup"><span data-stu-id="2c58f-124">The registry data detection type.</span></span> <span data-ttu-id="2c58f-125">可取值为：`notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。</span><span class="sxs-lookup"><span data-stu-id="2c58f-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="2c58f-126">operator</span><span class="sxs-lookup"><span data-stu-id="2c58f-126">operator</span></span>|[<span data-ttu-id="2c58f-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="2c58f-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="2c58f-128">注册表数据检测运算符。</span><span class="sxs-lookup"><span data-stu-id="2c58f-128">The operator for registry data detection.</span></span> <span data-ttu-id="2c58f-129">可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual`。</span><span class="sxs-lookup"><span data-stu-id="2c58f-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="2c58f-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="2c58f-130">detectionValue</span></span>|<span data-ttu-id="2c58f-131">字符串</span><span class="sxs-lookup"><span data-stu-id="2c58f-131">String</span></span>|<span data-ttu-id="2c58f-132">注册表检测值</span><span class="sxs-lookup"><span data-stu-id="2c58f-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c58f-133">Relationships</span><span class="sxs-lookup"><span data-stu-id="2c58f-133">Relationships</span></span>
<span data-ttu-id="2c58f-134">无</span><span class="sxs-lookup"><span data-stu-id="2c58f-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2c58f-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c58f-135">JSON Representation</span></span>
<span data-ttu-id="2c58f-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c58f-136">Here is a JSON representation of the resource.</span></span>
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





