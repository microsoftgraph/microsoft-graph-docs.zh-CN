---
title: deviceDetail 资源类型
description: 指示与用于登录的设备的设备详细信息。 如果设备是托管的 Azure AD，包括设备的浏览器和操作系统信息等信息。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18d55e397cf6c892cd37aea930d446c630017a92
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971359"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="bd0ad-104">deviceDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="bd0ad-104">deviceDetail resource type</span></span>
<span data-ttu-id="bd0ad-105">指示与用于登录的设备的设备详细信息。</span><span class="sxs-lookup"><span data-stu-id="bd0ad-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="bd0ad-106">如果设备是托管的 Azure AD，包括设备的浏览器和操作系统信息等信息。</span><span class="sxs-lookup"><span data-stu-id="bd0ad-106">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="bd0ad-107">属性</span><span class="sxs-lookup"><span data-stu-id="bd0ad-107">Properties</span></span>
| <span data-ttu-id="bd0ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="bd0ad-108">Property</span></span>     | <span data-ttu-id="bd0ad-109">类型</span><span class="sxs-lookup"><span data-stu-id="bd0ad-109">Type</span></span>   |<span data-ttu-id="bd0ad-110">说明</span><span class="sxs-lookup"><span data-stu-id="bd0ad-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bd0ad-111">浏览器</span><span class="sxs-lookup"><span data-stu-id="bd0ad-111">browser</span></span>|<span data-ttu-id="bd0ad-112">字符串</span><span class="sxs-lookup"><span data-stu-id="bd0ad-112">String</span></span>|<span data-ttu-id="bd0ad-113">指示使用的浏览器信息签名项。</span><span class="sxs-lookup"><span data-stu-id="bd0ad-113">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="bd0ad-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="bd0ad-114">deviceId</span></span>|<span data-ttu-id="bd0ad-115">String</span><span class="sxs-lookup"><span data-stu-id="bd0ad-115">String</span></span>|<span data-ttu-id="bd0ad-116">指用于签名中的设备的 UniqueID。</span><span class="sxs-lookup"><span data-stu-id="bd0ad-116">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="bd0ad-117">displayName</span><span class="sxs-lookup"><span data-stu-id="bd0ad-117">displayName</span></span>|<span data-ttu-id="bd0ad-118">字符串</span><span class="sxs-lookup"><span data-stu-id="bd0ad-118">String</span></span>|<span data-ttu-id="bd0ad-119">指用于签名中的设备的名称。</span><span class="sxs-lookup"><span data-stu-id="bd0ad-119">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="bd0ad-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="bd0ad-120">isCompliant</span></span>|<span data-ttu-id="bd0ad-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd0ad-121">Boolean</span></span>|<span data-ttu-id="bd0ad-122">指示是否符合设备。</span><span class="sxs-lookup"><span data-stu-id="bd0ad-122">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="bd0ad-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="bd0ad-123">isManaged</span></span>|<span data-ttu-id="bd0ad-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd0ad-124">Boolean</span></span>|<span data-ttu-id="bd0ad-125">指示托管设备。</span><span class="sxs-lookup"><span data-stu-id="bd0ad-125">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="bd0ad-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="bd0ad-126">operatingSystem</span></span>|<span data-ttu-id="bd0ad-127">String</span><span class="sxs-lookup"><span data-stu-id="bd0ad-127">String</span></span>|<span data-ttu-id="bd0ad-128">指示 OS 名称和用于签名中的版本。</span><span class="sxs-lookup"><span data-stu-id="bd0ad-128">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="bd0ad-129">trustType</span><span class="sxs-lookup"><span data-stu-id="bd0ad-129">trustType</span></span>|<span data-ttu-id="bd0ad-130">String</span><span class="sxs-lookup"><span data-stu-id="bd0ad-130">String</span></span>|<span data-ttu-id="bd0ad-131">指示是否已登录的设备上工作场所加入，AzureAD 加入，加入域的信息。</span><span class="sxs-lookup"><span data-stu-id="bd0ad-131">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bd0ad-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bd0ad-132">JSON representation</span></span>

<span data-ttu-id="bd0ad-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd0ad-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "browser": "String",
  "deviceId": "String",
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "operatingSystem": "String",
  "trustType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
