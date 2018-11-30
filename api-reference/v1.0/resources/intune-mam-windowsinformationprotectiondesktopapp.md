---
title: windowsInformationProtectionDesktopApp 资源类型
description: 用于 Windows 信息保护的桌面应用
ms.openlocfilehash: b685304a52818dfdf982cb48739965aa3b018a63
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010596"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="65ad9-103">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="65ad9-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="65ad9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="65ad9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="65ad9-105">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="65ad9-105">Desktop App for Windows information protection</span></span>

<span data-ttu-id="65ad9-106">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="65ad9-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65ad9-107">属性</span><span class="sxs-lookup"><span data-stu-id="65ad9-107">Properties</span></span>
|<span data-ttu-id="65ad9-108">属性</span><span class="sxs-lookup"><span data-stu-id="65ad9-108">Property</span></span>|<span data-ttu-id="65ad9-109">类型</span><span class="sxs-lookup"><span data-stu-id="65ad9-109">Type</span></span>|<span data-ttu-id="65ad9-110">说明</span><span class="sxs-lookup"><span data-stu-id="65ad9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65ad9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="65ad9-111">displayName</span></span>|<span data-ttu-id="65ad9-112">String</span><span class="sxs-lookup"><span data-stu-id="65ad9-112">String</span></span>|<span data-ttu-id="65ad9-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="65ad9-113">App display name.</span></span> <span data-ttu-id="65ad9-114">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="65ad9-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="65ad9-115">description</span><span class="sxs-lookup"><span data-stu-id="65ad9-115">description</span></span>|<span data-ttu-id="65ad9-116">String</span><span class="sxs-lookup"><span data-stu-id="65ad9-116">String</span></span>|<span data-ttu-id="65ad9-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="65ad9-117">The app's description.</span></span> <span data-ttu-id="65ad9-118">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="65ad9-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="65ad9-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="65ad9-119">publisherName</span></span>|<span data-ttu-id="65ad9-120">String</span><span class="sxs-lookup"><span data-stu-id="65ad9-120">String</span></span>|<span data-ttu-id="65ad9-121">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="65ad9-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="65ad9-122">productName</span><span class="sxs-lookup"><span data-stu-id="65ad9-122">productName</span></span>|<span data-ttu-id="65ad9-123">String</span><span class="sxs-lookup"><span data-stu-id="65ad9-123">String</span></span>|<span data-ttu-id="65ad9-124">产品名称。</span><span class="sxs-lookup"><span data-stu-id="65ad9-124">The product name.</span></span> <span data-ttu-id="65ad9-125">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="65ad9-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="65ad9-126">denied</span><span class="sxs-lookup"><span data-stu-id="65ad9-126">denied</span></span>|<span data-ttu-id="65ad9-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="65ad9-127">Boolean</span></span>|<span data-ttu-id="65ad9-128">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="65ad9-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="65ad9-129">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="65ad9-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="65ad9-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="65ad9-130">binaryName</span></span>|<span data-ttu-id="65ad9-131">String</span><span class="sxs-lookup"><span data-stu-id="65ad9-131">String</span></span>|<span data-ttu-id="65ad9-132">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="65ad9-132">The binary name.</span></span>|
|<span data-ttu-id="65ad9-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="65ad9-133">binaryVersionLow</span></span>|<span data-ttu-id="65ad9-134">String</span><span class="sxs-lookup"><span data-stu-id="65ad9-134">String</span></span>|<span data-ttu-id="65ad9-135">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="65ad9-135">The lower binary version.</span></span>|
|<span data-ttu-id="65ad9-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="65ad9-136">binaryVersionHigh</span></span>|<span data-ttu-id="65ad9-137">String</span><span class="sxs-lookup"><span data-stu-id="65ad9-137">String</span></span>|<span data-ttu-id="65ad9-138">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="65ad9-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65ad9-139">关系</span><span class="sxs-lookup"><span data-stu-id="65ad9-139">Relationships</span></span>
<span data-ttu-id="65ad9-140">无</span><span class="sxs-lookup"><span data-stu-id="65ad9-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="65ad9-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65ad9-141">JSON Representation</span></span>
<span data-ttu-id="65ad9-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65ad9-142">Here is a JSON representation of the resource.</span></span>
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



