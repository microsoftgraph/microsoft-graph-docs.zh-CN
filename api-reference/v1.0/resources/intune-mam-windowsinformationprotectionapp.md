---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 250542a7ff87b02ee271c0fbb8682f9855cc24ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833934"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="840b3-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="840b3-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="840b3-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="840b3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="840b3-105">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="840b3-105">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="840b3-106">属性</span><span class="sxs-lookup"><span data-stu-id="840b3-106">Properties</span></span>
|<span data-ttu-id="840b3-107">属性</span><span class="sxs-lookup"><span data-stu-id="840b3-107">Property</span></span>|<span data-ttu-id="840b3-108">类型</span><span class="sxs-lookup"><span data-stu-id="840b3-108">Type</span></span>|<span data-ttu-id="840b3-109">说明</span><span class="sxs-lookup"><span data-stu-id="840b3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="840b3-110">displayName</span><span class="sxs-lookup"><span data-stu-id="840b3-110">displayName</span></span>|<span data-ttu-id="840b3-111">String</span><span class="sxs-lookup"><span data-stu-id="840b3-111">String</span></span>|<span data-ttu-id="840b3-112">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="840b3-112">App display name.</span></span>|
|<span data-ttu-id="840b3-113">description</span><span class="sxs-lookup"><span data-stu-id="840b3-113">description</span></span>|<span data-ttu-id="840b3-114">String</span><span class="sxs-lookup"><span data-stu-id="840b3-114">String</span></span>|<span data-ttu-id="840b3-115">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="840b3-115">The app's description.</span></span>|
|<span data-ttu-id="840b3-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="840b3-116">publisherName</span></span>|<span data-ttu-id="840b3-117">String</span><span class="sxs-lookup"><span data-stu-id="840b3-117">String</span></span>|<span data-ttu-id="840b3-118">发布者名称</span><span class="sxs-lookup"><span data-stu-id="840b3-118">The publisher name</span></span>|
|<span data-ttu-id="840b3-119">productName</span><span class="sxs-lookup"><span data-stu-id="840b3-119">productName</span></span>|<span data-ttu-id="840b3-120">String</span><span class="sxs-lookup"><span data-stu-id="840b3-120">String</span></span>|<span data-ttu-id="840b3-121">产品名称。</span><span class="sxs-lookup"><span data-stu-id="840b3-121">The product name.</span></span>|
|<span data-ttu-id="840b3-122">denied</span><span class="sxs-lookup"><span data-stu-id="840b3-122">denied</span></span>|<span data-ttu-id="840b3-123">布尔值</span><span class="sxs-lookup"><span data-stu-id="840b3-123">Boolean</span></span>|<span data-ttu-id="840b3-124">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="840b3-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="840b3-125">关系</span><span class="sxs-lookup"><span data-stu-id="840b3-125">Relationships</span></span>
<span data-ttu-id="840b3-126">无</span><span class="sxs-lookup"><span data-stu-id="840b3-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="840b3-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="840b3-127">JSON Representation</span></span>
<span data-ttu-id="840b3-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="840b3-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



