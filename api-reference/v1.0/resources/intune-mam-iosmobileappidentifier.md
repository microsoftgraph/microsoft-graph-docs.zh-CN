---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 088f5507051676d587334966b91d4d4d1e8a135c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468560"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="7f602-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f602-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="7f602-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f602-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f602-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f602-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f602-106">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="7f602-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="7f602-107">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="7f602-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7f602-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f602-108">Properties</span></span>
|<span data-ttu-id="7f602-109">属性</span><span class="sxs-lookup"><span data-stu-id="7f602-109">Property</span></span>|<span data-ttu-id="7f602-110">类型</span><span class="sxs-lookup"><span data-stu-id="7f602-110">Type</span></span>|<span data-ttu-id="7f602-111">说明</span><span class="sxs-lookup"><span data-stu-id="7f602-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f602-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="7f602-112">bundleId</span></span>|<span data-ttu-id="7f602-113">String</span><span class="sxs-lookup"><span data-stu-id="7f602-113">String</span></span>|<span data-ttu-id="7f602-114">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="7f602-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f602-115">关系</span><span class="sxs-lookup"><span data-stu-id="7f602-115">Relationships</span></span>
<span data-ttu-id="7f602-116">无</span><span class="sxs-lookup"><span data-stu-id="7f602-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f602-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f602-117">JSON Representation</span></span>
<span data-ttu-id="7f602-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f602-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```







