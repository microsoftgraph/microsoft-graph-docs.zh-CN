---
title: windowsInformationProtectionStoreApp 资源类型
description: 用于 Windows 信息保护的应用商店应用
author: tfitzmac
ms.openlocfilehash: b5f13b77a5fbd9464ac968034fb19ae4e6327b9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344665"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="fc7f6-103">windowsInformationProtectionStoreApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc7f6-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="fc7f6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fc7f6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc7f6-105">用于 Windows 信息保护的应用商店应用</span><span class="sxs-lookup"><span data-stu-id="fc7f6-105">Store App for Windows information protection</span></span>

<span data-ttu-id="fc7f6-106">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7f6-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc7f6-107">属性</span><span class="sxs-lookup"><span data-stu-id="fc7f6-107">Properties</span></span>
|<span data-ttu-id="fc7f6-108">属性</span><span class="sxs-lookup"><span data-stu-id="fc7f6-108">Property</span></span>|<span data-ttu-id="fc7f6-109">类型</span><span class="sxs-lookup"><span data-stu-id="fc7f6-109">Type</span></span>|<span data-ttu-id="fc7f6-110">说明</span><span class="sxs-lookup"><span data-stu-id="fc7f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc7f6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="fc7f6-111">displayName</span></span>|<span data-ttu-id="fc7f6-112">String</span><span class="sxs-lookup"><span data-stu-id="fc7f6-112">String</span></span>|<span data-ttu-id="fc7f6-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="fc7f6-113">App display name.</span></span> <span data-ttu-id="fc7f6-114">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7f6-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="fc7f6-115">description</span><span class="sxs-lookup"><span data-stu-id="fc7f6-115">description</span></span>|<span data-ttu-id="fc7f6-116">String</span><span class="sxs-lookup"><span data-stu-id="fc7f6-116">String</span></span>|<span data-ttu-id="fc7f6-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="fc7f6-117">The app's description.</span></span> <span data-ttu-id="fc7f6-118">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7f6-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="fc7f6-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="fc7f6-119">publisherName</span></span>|<span data-ttu-id="fc7f6-120">String</span><span class="sxs-lookup"><span data-stu-id="fc7f6-120">String</span></span>|<span data-ttu-id="fc7f6-121">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="fc7f6-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="fc7f6-122">productName</span><span class="sxs-lookup"><span data-stu-id="fc7f6-122">productName</span></span>|<span data-ttu-id="fc7f6-123">String</span><span class="sxs-lookup"><span data-stu-id="fc7f6-123">String</span></span>|<span data-ttu-id="fc7f6-124">产品名称。</span><span class="sxs-lookup"><span data-stu-id="fc7f6-124">The product name.</span></span> <span data-ttu-id="fc7f6-125">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7f6-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="fc7f6-126">denied</span><span class="sxs-lookup"><span data-stu-id="fc7f6-126">denied</span></span>|<span data-ttu-id="fc7f6-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc7f6-127">Boolean</span></span>|<span data-ttu-id="fc7f6-128">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="fc7f6-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="fc7f6-129">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="fc7f6-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc7f6-130">关系</span><span class="sxs-lookup"><span data-stu-id="fc7f6-130">Relationships</span></span>
<span data-ttu-id="fc7f6-131">无</span><span class="sxs-lookup"><span data-stu-id="fc7f6-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fc7f6-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc7f6-132">JSON Representation</span></span>
<span data-ttu-id="fc7f6-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc7f6-133">Here is a JSON representation of the resource.</span></span>
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



