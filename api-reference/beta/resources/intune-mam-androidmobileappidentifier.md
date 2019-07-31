---
title: androidMobileAppIdentifier 资源类型
description: Android 应用的标识符。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9000c2989dc9b8e41c1f9aa36a05c29fc7a86cfe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010903"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="ce293-103">androidMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce293-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="ce293-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ce293-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce293-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce293-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce293-106">Android 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="ce293-106">The identifier for an Android app.</span></span>


<span data-ttu-id="ce293-107">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="ce293-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ce293-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce293-108">Properties</span></span>
|<span data-ttu-id="ce293-109">属性</span><span class="sxs-lookup"><span data-stu-id="ce293-109">Property</span></span>|<span data-ttu-id="ce293-110">类型</span><span class="sxs-lookup"><span data-stu-id="ce293-110">Type</span></span>|<span data-ttu-id="ce293-111">说明</span><span class="sxs-lookup"><span data-stu-id="ce293-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce293-112">packageId</span><span class="sxs-lookup"><span data-stu-id="ce293-112">packageId</span></span>|<span data-ttu-id="ce293-113">String</span><span class="sxs-lookup"><span data-stu-id="ce293-113">String</span></span>|<span data-ttu-id="ce293-114">应用的标识符，如 Play 商店中指定。</span><span class="sxs-lookup"><span data-stu-id="ce293-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce293-115">关系</span><span class="sxs-lookup"><span data-stu-id="ce293-115">Relationships</span></span>
<span data-ttu-id="ce293-116">无</span><span class="sxs-lookup"><span data-stu-id="ce293-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce293-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce293-117">JSON Representation</span></span>
<span data-ttu-id="ce293-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce293-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```





