---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 97e1e866dc71b08064fe46878c25cb5b43c90177
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533330"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="bc86e-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="bc86e-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="bc86e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc86e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bc86e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bc86e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc86e-106">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="bc86e-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="bc86e-107">属性</span><span class="sxs-lookup"><span data-stu-id="bc86e-107">Properties</span></span>
|<span data-ttu-id="bc86e-108">属性</span><span class="sxs-lookup"><span data-stu-id="bc86e-108">Property</span></span>|<span data-ttu-id="bc86e-109">类型</span><span class="sxs-lookup"><span data-stu-id="bc86e-109">Type</span></span>|<span data-ttu-id="bc86e-110">说明</span><span class="sxs-lookup"><span data-stu-id="bc86e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc86e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="bc86e-111">displayName</span></span>|<span data-ttu-id="bc86e-112">字符串</span><span class="sxs-lookup"><span data-stu-id="bc86e-112">String</span></span>|<span data-ttu-id="bc86e-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="bc86e-113">App display name.</span></span>|
|<span data-ttu-id="bc86e-114">说明</span><span class="sxs-lookup"><span data-stu-id="bc86e-114">description</span></span>|<span data-ttu-id="bc86e-115">字符串</span><span class="sxs-lookup"><span data-stu-id="bc86e-115">String</span></span>|<span data-ttu-id="bc86e-116">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="bc86e-116">The app's description.</span></span>|
|<span data-ttu-id="bc86e-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="bc86e-117">publisherName</span></span>|<span data-ttu-id="bc86e-118">String</span><span class="sxs-lookup"><span data-stu-id="bc86e-118">String</span></span>|<span data-ttu-id="bc86e-119">发布者名称</span><span class="sxs-lookup"><span data-stu-id="bc86e-119">The publisher name</span></span>|
|<span data-ttu-id="bc86e-120">productName</span><span class="sxs-lookup"><span data-stu-id="bc86e-120">productName</span></span>|<span data-ttu-id="bc86e-121">String</span><span class="sxs-lookup"><span data-stu-id="bc86e-121">String</span></span>|<span data-ttu-id="bc86e-122">产品名称。</span><span class="sxs-lookup"><span data-stu-id="bc86e-122">The product name.</span></span>|
|<span data-ttu-id="bc86e-123">denied</span><span class="sxs-lookup"><span data-stu-id="bc86e-123">denied</span></span>|<span data-ttu-id="bc86e-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc86e-124">Boolean</span></span>|<span data-ttu-id="bc86e-125">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="bc86e-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc86e-126">关系</span><span class="sxs-lookup"><span data-stu-id="bc86e-126">Relationships</span></span>
<span data-ttu-id="bc86e-127">无</span><span class="sxs-lookup"><span data-stu-id="bc86e-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc86e-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc86e-128">JSON Representation</span></span>
<span data-ttu-id="bc86e-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc86e-129">Here is a JSON representation of the resource.</span></span>
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




