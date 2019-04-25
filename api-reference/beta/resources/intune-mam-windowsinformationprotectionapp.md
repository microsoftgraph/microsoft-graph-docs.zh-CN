---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb14092fa9f347e551a4871da69d9a3631b96e8c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579175"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="bf0f4-103">windowsInformationProtectionApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf0f4-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="bf0f4-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf0f4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf0f4-106">用于 Windows 信息保护的应用</span><span class="sxs-lookup"><span data-stu-id="bf0f4-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="bf0f4-107">属性</span><span class="sxs-lookup"><span data-stu-id="bf0f4-107">Properties</span></span>
|<span data-ttu-id="bf0f4-108">属性</span><span class="sxs-lookup"><span data-stu-id="bf0f4-108">Property</span></span>|<span data-ttu-id="bf0f4-109">类型</span><span class="sxs-lookup"><span data-stu-id="bf0f4-109">Type</span></span>|<span data-ttu-id="bf0f4-110">说明</span><span class="sxs-lookup"><span data-stu-id="bf0f4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf0f4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="bf0f4-111">displayName</span></span>|<span data-ttu-id="bf0f4-112">字符串</span><span class="sxs-lookup"><span data-stu-id="bf0f4-112">String</span></span>|<span data-ttu-id="bf0f4-113">应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-113">App display name.</span></span>|
|<span data-ttu-id="bf0f4-114">说明</span><span class="sxs-lookup"><span data-stu-id="bf0f4-114">description</span></span>|<span data-ttu-id="bf0f4-115">String</span><span class="sxs-lookup"><span data-stu-id="bf0f4-115">String</span></span>|<span data-ttu-id="bf0f4-116">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-116">The app's description.</span></span>|
|<span data-ttu-id="bf0f4-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="bf0f4-117">publisherName</span></span>|<span data-ttu-id="bf0f4-118">String</span><span class="sxs-lookup"><span data-stu-id="bf0f4-118">String</span></span>|<span data-ttu-id="bf0f4-119">发布者名称</span><span class="sxs-lookup"><span data-stu-id="bf0f4-119">The publisher name</span></span>|
|<span data-ttu-id="bf0f4-120">productName</span><span class="sxs-lookup"><span data-stu-id="bf0f4-120">productName</span></span>|<span data-ttu-id="bf0f4-121">String</span><span class="sxs-lookup"><span data-stu-id="bf0f4-121">String</span></span>|<span data-ttu-id="bf0f4-122">产品名称。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-122">The product name.</span></span>|
|<span data-ttu-id="bf0f4-123">denied</span><span class="sxs-lookup"><span data-stu-id="bf0f4-123">denied</span></span>|<span data-ttu-id="bf0f4-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf0f4-124">Boolean</span></span>|<span data-ttu-id="bf0f4-125">如果为 true，则应用的保护或免除受到拒绝。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf0f4-126">关系</span><span class="sxs-lookup"><span data-stu-id="bf0f4-126">Relationships</span></span>
<span data-ttu-id="bf0f4-127">无</span><span class="sxs-lookup"><span data-stu-id="bf0f4-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf0f4-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf0f4-128">JSON Representation</span></span>
<span data-ttu-id="bf0f4-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf0f4-129">Here is a JSON representation of the resource.</span></span>
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





