---
title: windowsInformationProtectionDesktopApp 资源类型
description: 用于 Windows 信息保护的桌面应用
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d570420512e9da31fcd95efd2df2c2a3e1da83c9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367306"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="febc0-103">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="febc0-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="febc0-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="febc0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="febc0-105">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="febc0-105">Desktop App for Windows information protection</span></span>


<span data-ttu-id="febc0-106">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="febc0-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="febc0-107">属性</span><span class="sxs-lookup"><span data-stu-id="febc0-107">Properties</span></span>
|<span data-ttu-id="febc0-108">属性</span><span class="sxs-lookup"><span data-stu-id="febc0-108">Property</span></span>|<span data-ttu-id="febc0-109">类型</span><span class="sxs-lookup"><span data-stu-id="febc0-109">Type</span></span>|<span data-ttu-id="febc0-110">说明</span><span class="sxs-lookup"><span data-stu-id="febc0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="febc0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="febc0-111">displayName</span></span>|<span data-ttu-id="febc0-112">字符串</span><span class="sxs-lookup"><span data-stu-id="febc0-112">String</span></span>|<span data-ttu-id="febc0-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="febc0-113">App display name.</span></span> <span data-ttu-id="febc0-114">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="febc0-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="febc0-115">说明</span><span class="sxs-lookup"><span data-stu-id="febc0-115">description</span></span>|<span data-ttu-id="febc0-116">字符串</span><span class="sxs-lookup"><span data-stu-id="febc0-116">String</span></span>|<span data-ttu-id="febc0-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="febc0-117">The app's description.</span></span> <span data-ttu-id="febc0-118">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="febc0-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="febc0-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="febc0-119">publisherName</span></span>|<span data-ttu-id="febc0-120">String</span><span class="sxs-lookup"><span data-stu-id="febc0-120">String</span></span>|<span data-ttu-id="febc0-121">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="febc0-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="febc0-122">productName</span><span class="sxs-lookup"><span data-stu-id="febc0-122">productName</span></span>|<span data-ttu-id="febc0-123">String</span><span class="sxs-lookup"><span data-stu-id="febc0-123">String</span></span>|<span data-ttu-id="febc0-124">产品名称。</span><span class="sxs-lookup"><span data-stu-id="febc0-124">The product name.</span></span> <span data-ttu-id="febc0-125">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="febc0-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="febc0-126">denied</span><span class="sxs-lookup"><span data-stu-id="febc0-126">denied</span></span>|<span data-ttu-id="febc0-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="febc0-127">Boolean</span></span>|<span data-ttu-id="febc0-128">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="febc0-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="febc0-129">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="febc0-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="febc0-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="febc0-130">binaryName</span></span>|<span data-ttu-id="febc0-131">String</span><span class="sxs-lookup"><span data-stu-id="febc0-131">String</span></span>|<span data-ttu-id="febc0-132">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="febc0-132">The binary name.</span></span>|
|<span data-ttu-id="febc0-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="febc0-133">binaryVersionLow</span></span>|<span data-ttu-id="febc0-134">String</span><span class="sxs-lookup"><span data-stu-id="febc0-134">String</span></span>|<span data-ttu-id="febc0-135">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="febc0-135">The lower binary version.</span></span>|
|<span data-ttu-id="febc0-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="febc0-136">binaryVersionHigh</span></span>|<span data-ttu-id="febc0-137">String</span><span class="sxs-lookup"><span data-stu-id="febc0-137">String</span></span>|<span data-ttu-id="febc0-138">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="febc0-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="febc0-139">关系</span><span class="sxs-lookup"><span data-stu-id="febc0-139">Relationships</span></span>
<span data-ttu-id="febc0-140">无</span><span class="sxs-lookup"><span data-stu-id="febc0-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="febc0-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="febc0-141">JSON Representation</span></span>
<span data-ttu-id="febc0-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="febc0-142">Here is a JSON representation of the resource.</span></span>
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




