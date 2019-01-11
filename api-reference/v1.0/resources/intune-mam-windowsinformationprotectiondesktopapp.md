---
title: windowsInformationProtectionDesktopApp 资源类型
description: 用于 Windows 信息保护的桌面应用
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c381541379feacff7611e77882069c5fe2119e67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822062"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="b627f-103">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="b627f-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="b627f-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b627f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b627f-105">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="b627f-105">Desktop App for Windows information protection</span></span>

<span data-ttu-id="b627f-106">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b627f-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b627f-107">属性</span><span class="sxs-lookup"><span data-stu-id="b627f-107">Properties</span></span>
|<span data-ttu-id="b627f-108">属性</span><span class="sxs-lookup"><span data-stu-id="b627f-108">Property</span></span>|<span data-ttu-id="b627f-109">类型</span><span class="sxs-lookup"><span data-stu-id="b627f-109">Type</span></span>|<span data-ttu-id="b627f-110">说明</span><span class="sxs-lookup"><span data-stu-id="b627f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b627f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b627f-111">displayName</span></span>|<span data-ttu-id="b627f-112">String</span><span class="sxs-lookup"><span data-stu-id="b627f-112">String</span></span>|<span data-ttu-id="b627f-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="b627f-113">App display name.</span></span> <span data-ttu-id="b627f-114">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b627f-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b627f-115">description</span><span class="sxs-lookup"><span data-stu-id="b627f-115">description</span></span>|<span data-ttu-id="b627f-116">String</span><span class="sxs-lookup"><span data-stu-id="b627f-116">String</span></span>|<span data-ttu-id="b627f-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="b627f-117">The app's description.</span></span> <span data-ttu-id="b627f-118">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b627f-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b627f-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="b627f-119">publisherName</span></span>|<span data-ttu-id="b627f-120">String</span><span class="sxs-lookup"><span data-stu-id="b627f-120">String</span></span>|<span data-ttu-id="b627f-121">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="b627f-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b627f-122">productName</span><span class="sxs-lookup"><span data-stu-id="b627f-122">productName</span></span>|<span data-ttu-id="b627f-123">String</span><span class="sxs-lookup"><span data-stu-id="b627f-123">String</span></span>|<span data-ttu-id="b627f-124">产品名称。</span><span class="sxs-lookup"><span data-stu-id="b627f-124">The product name.</span></span> <span data-ttu-id="b627f-125">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b627f-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b627f-126">denied</span><span class="sxs-lookup"><span data-stu-id="b627f-126">denied</span></span>|<span data-ttu-id="b627f-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="b627f-127">Boolean</span></span>|<span data-ttu-id="b627f-128">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="b627f-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="b627f-129">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="b627f-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="b627f-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="b627f-130">binaryName</span></span>|<span data-ttu-id="b627f-131">String</span><span class="sxs-lookup"><span data-stu-id="b627f-131">String</span></span>|<span data-ttu-id="b627f-132">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="b627f-132">The binary name.</span></span>|
|<span data-ttu-id="b627f-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="b627f-133">binaryVersionLow</span></span>|<span data-ttu-id="b627f-134">String</span><span class="sxs-lookup"><span data-stu-id="b627f-134">String</span></span>|<span data-ttu-id="b627f-135">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="b627f-135">The lower binary version.</span></span>|
|<span data-ttu-id="b627f-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="b627f-136">binaryVersionHigh</span></span>|<span data-ttu-id="b627f-137">String</span><span class="sxs-lookup"><span data-stu-id="b627f-137">String</span></span>|<span data-ttu-id="b627f-138">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="b627f-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b627f-139">关系</span><span class="sxs-lookup"><span data-stu-id="b627f-139">Relationships</span></span>
<span data-ttu-id="b627f-140">无</span><span class="sxs-lookup"><span data-stu-id="b627f-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b627f-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b627f-141">JSON Representation</span></span>
<span data-ttu-id="b627f-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b627f-142">Here is a JSON representation of the resource.</span></span>
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



