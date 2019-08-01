---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 32dd1213bb06fbaa80a744d78453b12f6eeff7dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037756"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="430bb-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="430bb-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="430bb-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="430bb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="430bb-105">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="430bb-105">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="430bb-106">属性</span><span class="sxs-lookup"><span data-stu-id="430bb-106">Properties</span></span>
|<span data-ttu-id="430bb-107">属性</span><span class="sxs-lookup"><span data-stu-id="430bb-107">Property</span></span>|<span data-ttu-id="430bb-108">类型</span><span class="sxs-lookup"><span data-stu-id="430bb-108">Type</span></span>|<span data-ttu-id="430bb-109">说明</span><span class="sxs-lookup"><span data-stu-id="430bb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="430bb-110">displayName</span><span class="sxs-lookup"><span data-stu-id="430bb-110">displayName</span></span>|<span data-ttu-id="430bb-111">字符串</span><span class="sxs-lookup"><span data-stu-id="430bb-111">String</span></span>|<span data-ttu-id="430bb-112">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="430bb-112">App display name.</span></span>|
|<span data-ttu-id="430bb-113">说明</span><span class="sxs-lookup"><span data-stu-id="430bb-113">description</span></span>|<span data-ttu-id="430bb-114">字符串</span><span class="sxs-lookup"><span data-stu-id="430bb-114">String</span></span>|<span data-ttu-id="430bb-115">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="430bb-115">The app's description.</span></span>|
|<span data-ttu-id="430bb-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="430bb-116">publisherName</span></span>|<span data-ttu-id="430bb-117">String</span><span class="sxs-lookup"><span data-stu-id="430bb-117">String</span></span>|<span data-ttu-id="430bb-118">发布者名称</span><span class="sxs-lookup"><span data-stu-id="430bb-118">The publisher name</span></span>|
|<span data-ttu-id="430bb-119">productName</span><span class="sxs-lookup"><span data-stu-id="430bb-119">productName</span></span>|<span data-ttu-id="430bb-120">String</span><span class="sxs-lookup"><span data-stu-id="430bb-120">String</span></span>|<span data-ttu-id="430bb-121">产品名称。</span><span class="sxs-lookup"><span data-stu-id="430bb-121">The product name.</span></span>|
|<span data-ttu-id="430bb-122">denied</span><span class="sxs-lookup"><span data-stu-id="430bb-122">denied</span></span>|<span data-ttu-id="430bb-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="430bb-123">Boolean</span></span>|<span data-ttu-id="430bb-124">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="430bb-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="430bb-125">关系</span><span class="sxs-lookup"><span data-stu-id="430bb-125">Relationships</span></span>
<span data-ttu-id="430bb-126">无</span><span class="sxs-lookup"><span data-stu-id="430bb-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="430bb-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="430bb-127">JSON Representation</span></span>
<span data-ttu-id="430bb-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="430bb-128">Here is a JSON representation of the resource.</span></span>
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



