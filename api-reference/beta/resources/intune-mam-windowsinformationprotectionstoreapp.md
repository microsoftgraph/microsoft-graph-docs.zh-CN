---
title: windowsInformationProtectionStoreApp 资源类型
description: 用于 Windows 信息保护的应用商店应用
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c389b9a8e529b549c537cba9c9f02b0f81879db6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42780330"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="61715-103">windowsInformationProtectionStoreApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="61715-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="61715-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="61715-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61715-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="61715-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61715-106">用于 Windows 信息保护的应用商店应用</span><span class="sxs-lookup"><span data-stu-id="61715-106">Store App for Windows information protection</span></span>


<span data-ttu-id="61715-107">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="61715-107">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="61715-108">属性</span><span class="sxs-lookup"><span data-stu-id="61715-108">Properties</span></span>
|<span data-ttu-id="61715-109">属性</span><span class="sxs-lookup"><span data-stu-id="61715-109">Property</span></span>|<span data-ttu-id="61715-110">类型</span><span class="sxs-lookup"><span data-stu-id="61715-110">Type</span></span>|<span data-ttu-id="61715-111">说明</span><span class="sxs-lookup"><span data-stu-id="61715-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61715-112">displayName</span><span class="sxs-lookup"><span data-stu-id="61715-112">displayName</span></span>|<span data-ttu-id="61715-113">字符串</span><span class="sxs-lookup"><span data-stu-id="61715-113">String</span></span>|<span data-ttu-id="61715-114">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="61715-114">App display name.</span></span> <span data-ttu-id="61715-115">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="61715-115">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="61715-116">说明</span><span class="sxs-lookup"><span data-stu-id="61715-116">description</span></span>|<span data-ttu-id="61715-117">字符串</span><span class="sxs-lookup"><span data-stu-id="61715-117">String</span></span>|<span data-ttu-id="61715-118">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="61715-118">The app's description.</span></span> <span data-ttu-id="61715-119">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="61715-119">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="61715-120">publisherName</span><span class="sxs-lookup"><span data-stu-id="61715-120">publisherName</span></span>|<span data-ttu-id="61715-121">String</span><span class="sxs-lookup"><span data-stu-id="61715-121">String</span></span>|<span data-ttu-id="61715-122">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="61715-122">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="61715-123">productName</span><span class="sxs-lookup"><span data-stu-id="61715-123">productName</span></span>|<span data-ttu-id="61715-124">String</span><span class="sxs-lookup"><span data-stu-id="61715-124">String</span></span>|<span data-ttu-id="61715-125">产品名称。</span><span class="sxs-lookup"><span data-stu-id="61715-125">The product name.</span></span> <span data-ttu-id="61715-126">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="61715-126">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="61715-127">denied</span><span class="sxs-lookup"><span data-stu-id="61715-127">denied</span></span>|<span data-ttu-id="61715-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="61715-128">Boolean</span></span>|<span data-ttu-id="61715-129">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="61715-129">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="61715-130">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="61715-130">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="61715-131">关系</span><span class="sxs-lookup"><span data-stu-id="61715-131">Relationships</span></span>
<span data-ttu-id="61715-132">无</span><span class="sxs-lookup"><span data-stu-id="61715-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61715-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61715-133">JSON Representation</span></span>
<span data-ttu-id="61715-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61715-134">Here is a JSON representation of the resource.</span></span>
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



