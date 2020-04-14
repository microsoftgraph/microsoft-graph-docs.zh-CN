---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b255fdc604c5b1aacc4c7cbfd5750b01675fe335
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43443758"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="96a73-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="96a73-103">windowsInformationProtectionApp resource type</span></span>

<span data-ttu-id="96a73-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96a73-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96a73-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96a73-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96a73-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96a73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96a73-107">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="96a73-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="96a73-108">属性</span><span class="sxs-lookup"><span data-stu-id="96a73-108">Properties</span></span>
|<span data-ttu-id="96a73-109">属性</span><span class="sxs-lookup"><span data-stu-id="96a73-109">Property</span></span>|<span data-ttu-id="96a73-110">类型</span><span class="sxs-lookup"><span data-stu-id="96a73-110">Type</span></span>|<span data-ttu-id="96a73-111">说明</span><span class="sxs-lookup"><span data-stu-id="96a73-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96a73-112">displayName</span><span class="sxs-lookup"><span data-stu-id="96a73-112">displayName</span></span>|<span data-ttu-id="96a73-113">字符串</span><span class="sxs-lookup"><span data-stu-id="96a73-113">String</span></span>|<span data-ttu-id="96a73-114">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="96a73-114">App display name.</span></span>|
|<span data-ttu-id="96a73-115">description</span><span class="sxs-lookup"><span data-stu-id="96a73-115">description</span></span>|<span data-ttu-id="96a73-116">字符串</span><span class="sxs-lookup"><span data-stu-id="96a73-116">String</span></span>|<span data-ttu-id="96a73-117">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="96a73-117">The app's description.</span></span>|
|<span data-ttu-id="96a73-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="96a73-118">publisherName</span></span>|<span data-ttu-id="96a73-119">String</span><span class="sxs-lookup"><span data-stu-id="96a73-119">String</span></span>|<span data-ttu-id="96a73-120">发布者名称</span><span class="sxs-lookup"><span data-stu-id="96a73-120">The publisher name</span></span>|
|<span data-ttu-id="96a73-121">productName</span><span class="sxs-lookup"><span data-stu-id="96a73-121">productName</span></span>|<span data-ttu-id="96a73-122">String</span><span class="sxs-lookup"><span data-stu-id="96a73-122">String</span></span>|<span data-ttu-id="96a73-123">产品名称。</span><span class="sxs-lookup"><span data-stu-id="96a73-123">The product name.</span></span>|
|<span data-ttu-id="96a73-124">denied</span><span class="sxs-lookup"><span data-stu-id="96a73-124">denied</span></span>|<span data-ttu-id="96a73-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="96a73-125">Boolean</span></span>|<span data-ttu-id="96a73-126">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="96a73-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96a73-127">关系</span><span class="sxs-lookup"><span data-stu-id="96a73-127">Relationships</span></span>
<span data-ttu-id="96a73-128">无</span><span class="sxs-lookup"><span data-stu-id="96a73-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96a73-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96a73-129">JSON Representation</span></span>
<span data-ttu-id="96a73-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96a73-130">Here is a JSON representation of the resource.</span></span>
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



