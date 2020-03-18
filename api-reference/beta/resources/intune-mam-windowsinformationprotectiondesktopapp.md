---
title: windowsInformationProtectionDesktopApp 资源类型
description: 用于 Windows 信息保护的桌面应用
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 44aa52bfe2dbae82adfc98c49fbba5a1aae500bf
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42780785"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="be140-103">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="be140-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="be140-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="be140-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be140-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be140-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be140-106">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="be140-106">Desktop App for Windows information protection</span></span>


<span data-ttu-id="be140-107">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="be140-107">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="be140-108">属性</span><span class="sxs-lookup"><span data-stu-id="be140-108">Properties</span></span>
|<span data-ttu-id="be140-109">属性</span><span class="sxs-lookup"><span data-stu-id="be140-109">Property</span></span>|<span data-ttu-id="be140-110">类型</span><span class="sxs-lookup"><span data-stu-id="be140-110">Type</span></span>|<span data-ttu-id="be140-111">说明</span><span class="sxs-lookup"><span data-stu-id="be140-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be140-112">displayName</span><span class="sxs-lookup"><span data-stu-id="be140-112">displayName</span></span>|<span data-ttu-id="be140-113">字符串</span><span class="sxs-lookup"><span data-stu-id="be140-113">String</span></span>|<span data-ttu-id="be140-114">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="be140-114">App display name.</span></span> <span data-ttu-id="be140-115">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="be140-115">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="be140-116">说明</span><span class="sxs-lookup"><span data-stu-id="be140-116">description</span></span>|<span data-ttu-id="be140-117">字符串</span><span class="sxs-lookup"><span data-stu-id="be140-117">String</span></span>|<span data-ttu-id="be140-118">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="be140-118">The app's description.</span></span> <span data-ttu-id="be140-119">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="be140-119">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="be140-120">publisherName</span><span class="sxs-lookup"><span data-stu-id="be140-120">publisherName</span></span>|<span data-ttu-id="be140-121">String</span><span class="sxs-lookup"><span data-stu-id="be140-121">String</span></span>|<span data-ttu-id="be140-122">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="be140-122">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="be140-123">productName</span><span class="sxs-lookup"><span data-stu-id="be140-123">productName</span></span>|<span data-ttu-id="be140-124">String</span><span class="sxs-lookup"><span data-stu-id="be140-124">String</span></span>|<span data-ttu-id="be140-125">产品名称。</span><span class="sxs-lookup"><span data-stu-id="be140-125">The product name.</span></span> <span data-ttu-id="be140-126">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="be140-126">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="be140-127">denied</span><span class="sxs-lookup"><span data-stu-id="be140-127">denied</span></span>|<span data-ttu-id="be140-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="be140-128">Boolean</span></span>|<span data-ttu-id="be140-129">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="be140-129">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="be140-130">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="be140-130">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="be140-131">binaryName</span><span class="sxs-lookup"><span data-stu-id="be140-131">binaryName</span></span>|<span data-ttu-id="be140-132">String</span><span class="sxs-lookup"><span data-stu-id="be140-132">String</span></span>|<span data-ttu-id="be140-133">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="be140-133">The binary name.</span></span>|
|<span data-ttu-id="be140-134">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="be140-134">binaryVersionLow</span></span>|<span data-ttu-id="be140-135">String</span><span class="sxs-lookup"><span data-stu-id="be140-135">String</span></span>|<span data-ttu-id="be140-136">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="be140-136">The lower binary version.</span></span>|
|<span data-ttu-id="be140-137">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="be140-137">binaryVersionHigh</span></span>|<span data-ttu-id="be140-138">String</span><span class="sxs-lookup"><span data-stu-id="be140-138">String</span></span>|<span data-ttu-id="be140-139">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="be140-139">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be140-140">关系</span><span class="sxs-lookup"><span data-stu-id="be140-140">Relationships</span></span>
<span data-ttu-id="be140-141">无</span><span class="sxs-lookup"><span data-stu-id="be140-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be140-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be140-142">JSON Representation</span></span>
<span data-ttu-id="be140-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be140-143">Here is a JSON representation of the resource.</span></span>
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



