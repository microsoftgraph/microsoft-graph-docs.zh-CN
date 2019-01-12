---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8d025b20e5341c17f756e86bb6bb84faf92a61a3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971877"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="e1c96-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1c96-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="e1c96-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e1c96-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1c96-105">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="e1c96-105">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="e1c96-106">属性</span><span class="sxs-lookup"><span data-stu-id="e1c96-106">Properties</span></span>
|<span data-ttu-id="e1c96-107">属性</span><span class="sxs-lookup"><span data-stu-id="e1c96-107">Property</span></span>|<span data-ttu-id="e1c96-108">类型</span><span class="sxs-lookup"><span data-stu-id="e1c96-108">Type</span></span>|<span data-ttu-id="e1c96-109">说明</span><span class="sxs-lookup"><span data-stu-id="e1c96-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1c96-110">displayName</span><span class="sxs-lookup"><span data-stu-id="e1c96-110">displayName</span></span>|<span data-ttu-id="e1c96-111">String</span><span class="sxs-lookup"><span data-stu-id="e1c96-111">String</span></span>|<span data-ttu-id="e1c96-112">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="e1c96-112">App display name.</span></span>|
|<span data-ttu-id="e1c96-113">description</span><span class="sxs-lookup"><span data-stu-id="e1c96-113">description</span></span>|<span data-ttu-id="e1c96-114">String</span><span class="sxs-lookup"><span data-stu-id="e1c96-114">String</span></span>|<span data-ttu-id="e1c96-115">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="e1c96-115">The app's description.</span></span>|
|<span data-ttu-id="e1c96-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="e1c96-116">publisherName</span></span>|<span data-ttu-id="e1c96-117">String</span><span class="sxs-lookup"><span data-stu-id="e1c96-117">String</span></span>|<span data-ttu-id="e1c96-118">发布者名称</span><span class="sxs-lookup"><span data-stu-id="e1c96-118">The publisher name</span></span>|
|<span data-ttu-id="e1c96-119">productName</span><span class="sxs-lookup"><span data-stu-id="e1c96-119">productName</span></span>|<span data-ttu-id="e1c96-120">String</span><span class="sxs-lookup"><span data-stu-id="e1c96-120">String</span></span>|<span data-ttu-id="e1c96-121">产品名称。</span><span class="sxs-lookup"><span data-stu-id="e1c96-121">The product name.</span></span>|
|<span data-ttu-id="e1c96-122">denied</span><span class="sxs-lookup"><span data-stu-id="e1c96-122">denied</span></span>|<span data-ttu-id="e1c96-123">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1c96-123">Boolean</span></span>|<span data-ttu-id="e1c96-124">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="e1c96-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1c96-125">关系</span><span class="sxs-lookup"><span data-stu-id="e1c96-125">Relationships</span></span>
<span data-ttu-id="e1c96-126">无</span><span class="sxs-lookup"><span data-stu-id="e1c96-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1c96-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1c96-127">JSON Representation</span></span>
<span data-ttu-id="e1c96-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1c96-128">Here is a JSON representation of the resource.</span></span>
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



