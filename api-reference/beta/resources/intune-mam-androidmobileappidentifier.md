---
title: androidMobileAppIdentifier 资源类型
description: Android 应用的标识符。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc998a09d30d94b42c6c118a51dc028b8251e134
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782662"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="d8df9-103">androidMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8df9-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="d8df9-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d8df9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8df9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8df9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8df9-106">Android 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="d8df9-106">The identifier for an Android app.</span></span>


<span data-ttu-id="d8df9-107">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="d8df9-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d8df9-108">属性</span><span class="sxs-lookup"><span data-stu-id="d8df9-108">Properties</span></span>
|<span data-ttu-id="d8df9-109">属性</span><span class="sxs-lookup"><span data-stu-id="d8df9-109">Property</span></span>|<span data-ttu-id="d8df9-110">类型</span><span class="sxs-lookup"><span data-stu-id="d8df9-110">Type</span></span>|<span data-ttu-id="d8df9-111">说明</span><span class="sxs-lookup"><span data-stu-id="d8df9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8df9-112">packageId</span><span class="sxs-lookup"><span data-stu-id="d8df9-112">packageId</span></span>|<span data-ttu-id="d8df9-113">String</span><span class="sxs-lookup"><span data-stu-id="d8df9-113">String</span></span>|<span data-ttu-id="d8df9-114">应用的标识符，如 Play 商店中指定。</span><span class="sxs-lookup"><span data-stu-id="d8df9-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8df9-115">关系</span><span class="sxs-lookup"><span data-stu-id="d8df9-115">Relationships</span></span>
<span data-ttu-id="d8df9-116">无</span><span class="sxs-lookup"><span data-stu-id="d8df9-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8df9-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8df9-117">JSON Representation</span></span>
<span data-ttu-id="d8df9-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8df9-118">Here is a JSON representation of the resource.</span></span>
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



