---
title: windowsInformationProtectionStoreApp 资源类型
description: 用于 Windows 信息保护的应用商店应用
ms.openlocfilehash: 3e175e1e3c01ddfe22341319e44005841d1619b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008372"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="6ab70-103">windowsInformationProtectionStoreApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ab70-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="6ab70-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6ab70-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ab70-105">用于 Windows 信息保护的应用商店应用</span><span class="sxs-lookup"><span data-stu-id="6ab70-105">Store App for Windows information protection</span></span>

<span data-ttu-id="6ab70-106">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="6ab70-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ab70-107">属性</span><span class="sxs-lookup"><span data-stu-id="6ab70-107">Properties</span></span>
|<span data-ttu-id="6ab70-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ab70-108">Property</span></span>|<span data-ttu-id="6ab70-109">类型</span><span class="sxs-lookup"><span data-stu-id="6ab70-109">Type</span></span>|<span data-ttu-id="6ab70-110">说明</span><span class="sxs-lookup"><span data-stu-id="6ab70-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ab70-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6ab70-111">displayName</span></span>|<span data-ttu-id="6ab70-112">String</span><span class="sxs-lookup"><span data-stu-id="6ab70-112">String</span></span>|<span data-ttu-id="6ab70-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="6ab70-113">App display name.</span></span> <span data-ttu-id="6ab70-114">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="6ab70-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6ab70-115">description</span><span class="sxs-lookup"><span data-stu-id="6ab70-115">description</span></span>|<span data-ttu-id="6ab70-116">String</span><span class="sxs-lookup"><span data-stu-id="6ab70-116">String</span></span>|<span data-ttu-id="6ab70-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="6ab70-117">The app's description.</span></span> <span data-ttu-id="6ab70-118">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="6ab70-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6ab70-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="6ab70-119">publisherName</span></span>|<span data-ttu-id="6ab70-120">String</span><span class="sxs-lookup"><span data-stu-id="6ab70-120">String</span></span>|<span data-ttu-id="6ab70-121">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="6ab70-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6ab70-122">productName</span><span class="sxs-lookup"><span data-stu-id="6ab70-122">productName</span></span>|<span data-ttu-id="6ab70-123">String</span><span class="sxs-lookup"><span data-stu-id="6ab70-123">String</span></span>|<span data-ttu-id="6ab70-124">产品名称。</span><span class="sxs-lookup"><span data-stu-id="6ab70-124">The product name.</span></span> <span data-ttu-id="6ab70-125">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="6ab70-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6ab70-126">denied</span><span class="sxs-lookup"><span data-stu-id="6ab70-126">denied</span></span>|<span data-ttu-id="6ab70-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="6ab70-127">Boolean</span></span>|<span data-ttu-id="6ab70-128">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="6ab70-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="6ab70-129">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="6ab70-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ab70-130">关系</span><span class="sxs-lookup"><span data-stu-id="6ab70-130">Relationships</span></span>
<span data-ttu-id="6ab70-131">无</span><span class="sxs-lookup"><span data-stu-id="6ab70-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ab70-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ab70-132">JSON Representation</span></span>
<span data-ttu-id="6ab70-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ab70-133">Here is a JSON representation of the resource.</span></span>
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



