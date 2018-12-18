---
title: windowsInformationProtectionDesktopApp 资源类型
description: 用于 Windows 信息保护的桌面应用
author: tfitzmac
ms.openlocfilehash: 5164e6d1a9165139de1895dfae38dd8c90927504
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345512"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="09e65-103">windowsInformationProtectionDesktopApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="09e65-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="09e65-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="09e65-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09e65-105">用于 Windows 信息保护的桌面应用</span><span class="sxs-lookup"><span data-stu-id="09e65-105">Desktop App for Windows information protection</span></span>

<span data-ttu-id="09e65-106">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="09e65-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09e65-107">属性</span><span class="sxs-lookup"><span data-stu-id="09e65-107">Properties</span></span>
|<span data-ttu-id="09e65-108">属性</span><span class="sxs-lookup"><span data-stu-id="09e65-108">Property</span></span>|<span data-ttu-id="09e65-109">类型</span><span class="sxs-lookup"><span data-stu-id="09e65-109">Type</span></span>|<span data-ttu-id="09e65-110">说明</span><span class="sxs-lookup"><span data-stu-id="09e65-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09e65-111">displayName</span><span class="sxs-lookup"><span data-stu-id="09e65-111">displayName</span></span>|<span data-ttu-id="09e65-112">String</span><span class="sxs-lookup"><span data-stu-id="09e65-112">String</span></span>|<span data-ttu-id="09e65-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="09e65-113">App display name.</span></span> <span data-ttu-id="09e65-114">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="09e65-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="09e65-115">description</span><span class="sxs-lookup"><span data-stu-id="09e65-115">description</span></span>|<span data-ttu-id="09e65-116">String</span><span class="sxs-lookup"><span data-stu-id="09e65-116">String</span></span>|<span data-ttu-id="09e65-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="09e65-117">The app's description.</span></span> <span data-ttu-id="09e65-118">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="09e65-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="09e65-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="09e65-119">publisherName</span></span>|<span data-ttu-id="09e65-120">String</span><span class="sxs-lookup"><span data-stu-id="09e65-120">String</span></span>|<span data-ttu-id="09e65-121">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="09e65-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="09e65-122">productName</span><span class="sxs-lookup"><span data-stu-id="09e65-122">productName</span></span>|<span data-ttu-id="09e65-123">String</span><span class="sxs-lookup"><span data-stu-id="09e65-123">String</span></span>|<span data-ttu-id="09e65-124">产品名称。</span><span class="sxs-lookup"><span data-stu-id="09e65-124">The product name.</span></span> <span data-ttu-id="09e65-125">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="09e65-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="09e65-126">denied</span><span class="sxs-lookup"><span data-stu-id="09e65-126">denied</span></span>|<span data-ttu-id="09e65-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="09e65-127">Boolean</span></span>|<span data-ttu-id="09e65-128">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="09e65-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="09e65-129">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="09e65-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="09e65-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="09e65-130">binaryName</span></span>|<span data-ttu-id="09e65-131">String</span><span class="sxs-lookup"><span data-stu-id="09e65-131">String</span></span>|<span data-ttu-id="09e65-132">二进制名称。</span><span class="sxs-lookup"><span data-stu-id="09e65-132">The binary name.</span></span>|
|<span data-ttu-id="09e65-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="09e65-133">binaryVersionLow</span></span>|<span data-ttu-id="09e65-134">String</span><span class="sxs-lookup"><span data-stu-id="09e65-134">String</span></span>|<span data-ttu-id="09e65-135">较低的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="09e65-135">The lower binary version.</span></span>|
|<span data-ttu-id="09e65-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="09e65-136">binaryVersionHigh</span></span>|<span data-ttu-id="09e65-137">String</span><span class="sxs-lookup"><span data-stu-id="09e65-137">String</span></span>|<span data-ttu-id="09e65-138">较高的二进制版本。</span><span class="sxs-lookup"><span data-stu-id="09e65-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09e65-139">关系</span><span class="sxs-lookup"><span data-stu-id="09e65-139">Relationships</span></span>
<span data-ttu-id="09e65-140">无</span><span class="sxs-lookup"><span data-stu-id="09e65-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09e65-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09e65-141">JSON Representation</span></span>
<span data-ttu-id="09e65-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09e65-142">Here is a JSON representation of the resource.</span></span>
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



