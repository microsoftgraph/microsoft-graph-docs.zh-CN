---
title: windowsInformationProtectionStoreApp 资源类型
description: 用于 Windows 信息保护的应用商店应用
ms.openlocfilehash: aff60cf420f4977d3869af3afcee624a080c686f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047435"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="eb6bc-103">windowsInformationProtectionStoreApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb6bc-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="eb6bc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eb6bc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb6bc-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eb6bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb6bc-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eb6bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb6bc-107">用于 Windows 信息保护的应用商店应用</span><span class="sxs-lookup"><span data-stu-id="eb6bc-107">Store App for Windows information protection</span></span>

<span data-ttu-id="eb6bc-108">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb6bc-108">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eb6bc-109">属性</span><span class="sxs-lookup"><span data-stu-id="eb6bc-109">Properties</span></span>
|<span data-ttu-id="eb6bc-110">属性</span><span class="sxs-lookup"><span data-stu-id="eb6bc-110">Property</span></span>|<span data-ttu-id="eb6bc-111">类型</span><span class="sxs-lookup"><span data-stu-id="eb6bc-111">Type</span></span>|<span data-ttu-id="eb6bc-112">说明</span><span class="sxs-lookup"><span data-stu-id="eb6bc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb6bc-113">displayName</span><span class="sxs-lookup"><span data-stu-id="eb6bc-113">displayName</span></span>|<span data-ttu-id="eb6bc-114">String</span><span class="sxs-lookup"><span data-stu-id="eb6bc-114">String</span></span>|<span data-ttu-id="eb6bc-115">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="eb6bc-115">App display name.</span></span> <span data-ttu-id="eb6bc-116">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb6bc-116">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb6bc-117">description</span><span class="sxs-lookup"><span data-stu-id="eb6bc-117">description</span></span>|<span data-ttu-id="eb6bc-118">String</span><span class="sxs-lookup"><span data-stu-id="eb6bc-118">String</span></span>|<span data-ttu-id="eb6bc-119">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="eb6bc-119">The app's description.</span></span> <span data-ttu-id="eb6bc-120">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb6bc-120">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb6bc-121">publisherName</span><span class="sxs-lookup"><span data-stu-id="eb6bc-121">publisherName</span></span>|<span data-ttu-id="eb6bc-122">String</span><span class="sxs-lookup"><span data-stu-id="eb6bc-122">String</span></span>|<span data-ttu-id="eb6bc-123">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) 的发布者名称</span><span class="sxs-lookup"><span data-stu-id="eb6bc-123">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb6bc-124">productName</span><span class="sxs-lookup"><span data-stu-id="eb6bc-124">productName</span></span>|<span data-ttu-id="eb6bc-125">String</span><span class="sxs-lookup"><span data-stu-id="eb6bc-125">String</span></span>|<span data-ttu-id="eb6bc-126">产品名称。</span><span class="sxs-lookup"><span data-stu-id="eb6bc-126">The product name.</span></span> <span data-ttu-id="eb6bc-127">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb6bc-127">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="eb6bc-128">denied</span><span class="sxs-lookup"><span data-stu-id="eb6bc-128">denied</span></span>|<span data-ttu-id="eb6bc-129">布尔值</span><span class="sxs-lookup"><span data-stu-id="eb6bc-129">Boolean</span></span>|<span data-ttu-id="eb6bc-130">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="eb6bc-130">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="eb6bc-131">继承自 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span><span class="sxs-lookup"><span data-stu-id="eb6bc-131">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb6bc-132">关系</span><span class="sxs-lookup"><span data-stu-id="eb6bc-132">Relationships</span></span>
<span data-ttu-id="eb6bc-133">无</span><span class="sxs-lookup"><span data-stu-id="eb6bc-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eb6bc-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb6bc-134">JSON Representation</span></span>
<span data-ttu-id="eb6bc-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb6bc-135">Here is a JSON representation of the resource.</span></span>
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





