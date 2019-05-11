---
title: windowsInformationProtectionStoreApp 资源类型
description: 用于 Windows 信息保护的应用商店应用
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 64310b1dd7924fbd77c67fd95dbb44958a163137
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940496"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="80057-103">windowsInformationProtectionStoreApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="80057-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="80057-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="80057-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80057-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80057-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80057-106">用于 Windows 信息保护的应用商店应用</span><span class="sxs-lookup"><span data-stu-id="80057-106">Store App for Windows information protection</span></span>


<span data-ttu-id="80057-107">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="80057-107">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="80057-108">属性</span><span class="sxs-lookup"><span data-stu-id="80057-108">Properties</span></span>
|<span data-ttu-id="80057-109">属性</span><span class="sxs-lookup"><span data-stu-id="80057-109">Property</span></span>|<span data-ttu-id="80057-110">类型</span><span class="sxs-lookup"><span data-stu-id="80057-110">Type</span></span>|<span data-ttu-id="80057-111">说明</span><span class="sxs-lookup"><span data-stu-id="80057-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80057-112">displayName</span><span class="sxs-lookup"><span data-stu-id="80057-112">displayName</span></span>|<span data-ttu-id="80057-113">字符串</span><span class="sxs-lookup"><span data-stu-id="80057-113">String</span></span>|<span data-ttu-id="80057-114">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="80057-114">App display name.</span></span> <span data-ttu-id="80057-115">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="80057-115">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="80057-116">说明</span><span class="sxs-lookup"><span data-stu-id="80057-116">description</span></span>|<span data-ttu-id="80057-117">字符串</span><span class="sxs-lookup"><span data-stu-id="80057-117">String</span></span>|<span data-ttu-id="80057-118">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="80057-118">The app's description.</span></span> <span data-ttu-id="80057-119">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="80057-119">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="80057-120">publisherName</span><span class="sxs-lookup"><span data-stu-id="80057-120">publisherName</span></span>|<span data-ttu-id="80057-121">String</span><span class="sxs-lookup"><span data-stu-id="80057-121">String</span></span>|<span data-ttu-id="80057-122">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="80057-122">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="80057-123">productName</span><span class="sxs-lookup"><span data-stu-id="80057-123">productName</span></span>|<span data-ttu-id="80057-124">String</span><span class="sxs-lookup"><span data-stu-id="80057-124">String</span></span>|<span data-ttu-id="80057-125">产品名称。</span><span class="sxs-lookup"><span data-stu-id="80057-125">The product name.</span></span> <span data-ttu-id="80057-126">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="80057-126">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="80057-127">denied</span><span class="sxs-lookup"><span data-stu-id="80057-127">denied</span></span>|<span data-ttu-id="80057-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="80057-128">Boolean</span></span>|<span data-ttu-id="80057-129">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="80057-129">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="80057-130">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="80057-130">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="80057-131">关系</span><span class="sxs-lookup"><span data-stu-id="80057-131">Relationships</span></span>
<span data-ttu-id="80057-132">无</span><span class="sxs-lookup"><span data-stu-id="80057-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80057-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80057-133">JSON Representation</span></span>
<span data-ttu-id="80057-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80057-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```




