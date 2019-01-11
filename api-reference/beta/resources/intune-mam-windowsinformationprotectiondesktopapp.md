---
title: windowsInformationProtectionDesktopApp 资源类型
description: 用于 Windows 信息保护的桌面应用
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2cfcca1f4ce8338c2fd7f894e6b0b7a23fbe66e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855263"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="386bf-103">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="386bf-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="386bf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="386bf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="386bf-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="386bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="386bf-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="386bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="386bf-107">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="386bf-107">Desktop App for Windows information protection</span></span>

<span data-ttu-id="386bf-108">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="386bf-108">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="386bf-109">属性</span><span class="sxs-lookup"><span data-stu-id="386bf-109">Properties</span></span>
|<span data-ttu-id="386bf-110">属性</span><span class="sxs-lookup"><span data-stu-id="386bf-110">Property</span></span>|<span data-ttu-id="386bf-111">类型</span><span class="sxs-lookup"><span data-stu-id="386bf-111">Type</span></span>|<span data-ttu-id="386bf-112">说明</span><span class="sxs-lookup"><span data-stu-id="386bf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="386bf-113">displayName</span><span class="sxs-lookup"><span data-stu-id="386bf-113">displayName</span></span>|<span data-ttu-id="386bf-114">String</span><span class="sxs-lookup"><span data-stu-id="386bf-114">String</span></span>|<span data-ttu-id="386bf-115">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="386bf-115">App display name.</span></span> <span data-ttu-id="386bf-116">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="386bf-116">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="386bf-117">description</span><span class="sxs-lookup"><span data-stu-id="386bf-117">description</span></span>|<span data-ttu-id="386bf-118">String</span><span class="sxs-lookup"><span data-stu-id="386bf-118">String</span></span>|<span data-ttu-id="386bf-119">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="386bf-119">The app's description.</span></span> <span data-ttu-id="386bf-120">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="386bf-120">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="386bf-121">publisherName</span><span class="sxs-lookup"><span data-stu-id="386bf-121">publisherName</span></span>|<span data-ttu-id="386bf-122">String</span><span class="sxs-lookup"><span data-stu-id="386bf-122">String</span></span>|<span data-ttu-id="386bf-123">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="386bf-123">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="386bf-124">productName</span><span class="sxs-lookup"><span data-stu-id="386bf-124">productName</span></span>|<span data-ttu-id="386bf-125">String</span><span class="sxs-lookup"><span data-stu-id="386bf-125">String</span></span>|<span data-ttu-id="386bf-126">产品名称。</span><span class="sxs-lookup"><span data-stu-id="386bf-126">The product name.</span></span> <span data-ttu-id="386bf-127">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="386bf-127">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="386bf-128">denied</span><span class="sxs-lookup"><span data-stu-id="386bf-128">denied</span></span>|<span data-ttu-id="386bf-129">布尔值</span><span class="sxs-lookup"><span data-stu-id="386bf-129">Boolean</span></span>|<span data-ttu-id="386bf-130">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="386bf-130">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="386bf-131">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="386bf-131">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="386bf-132">binaryName</span><span class="sxs-lookup"><span data-stu-id="386bf-132">binaryName</span></span>|<span data-ttu-id="386bf-133">String</span><span class="sxs-lookup"><span data-stu-id="386bf-133">String</span></span>|<span data-ttu-id="386bf-134">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="386bf-134">The binary name.</span></span>|
|<span data-ttu-id="386bf-135">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="386bf-135">binaryVersionLow</span></span>|<span data-ttu-id="386bf-136">String</span><span class="sxs-lookup"><span data-stu-id="386bf-136">String</span></span>|<span data-ttu-id="386bf-137">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="386bf-137">The lower binary version.</span></span>|
|<span data-ttu-id="386bf-138">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="386bf-138">binaryVersionHigh</span></span>|<span data-ttu-id="386bf-139">String</span><span class="sxs-lookup"><span data-stu-id="386bf-139">String</span></span>|<span data-ttu-id="386bf-140">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="386bf-140">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="386bf-141">关系</span><span class="sxs-lookup"><span data-stu-id="386bf-141">Relationships</span></span>
<span data-ttu-id="386bf-142">无</span><span class="sxs-lookup"><span data-stu-id="386bf-142">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="386bf-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="386bf-143">JSON Representation</span></span>
<span data-ttu-id="386bf-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="386bf-144">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```





