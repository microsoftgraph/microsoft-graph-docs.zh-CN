---
title: androidMobileAppIdentifier 资源类型
description: Android 应用的标识符。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7cbdaa159a07378776b141e4465b29d4880477b1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527999"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="1ff5c-103">androidMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="1ff5c-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="1ff5c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1ff5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ff5c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1ff5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ff5c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1ff5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ff5c-107">Android 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="1ff5c-107">The identifier for an Android app.</span></span>


<span data-ttu-id="1ff5c-108">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="1ff5c-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1ff5c-109">属性</span><span class="sxs-lookup"><span data-stu-id="1ff5c-109">Properties</span></span>
|<span data-ttu-id="1ff5c-110">属性</span><span class="sxs-lookup"><span data-stu-id="1ff5c-110">Property</span></span>|<span data-ttu-id="1ff5c-111">类型</span><span class="sxs-lookup"><span data-stu-id="1ff5c-111">Type</span></span>|<span data-ttu-id="1ff5c-112">说明</span><span class="sxs-lookup"><span data-stu-id="1ff5c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ff5c-113">packageId</span><span class="sxs-lookup"><span data-stu-id="1ff5c-113">packageId</span></span>|<span data-ttu-id="1ff5c-114">String</span><span class="sxs-lookup"><span data-stu-id="1ff5c-114">String</span></span>|<span data-ttu-id="1ff5c-115">应用的标识符，如 Play 商店中指定。</span><span class="sxs-lookup"><span data-stu-id="1ff5c-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ff5c-116">关系</span><span class="sxs-lookup"><span data-stu-id="1ff5c-116">Relationships</span></span>
<span data-ttu-id="1ff5c-117">无</span><span class="sxs-lookup"><span data-stu-id="1ff5c-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ff5c-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1ff5c-118">JSON Representation</span></span>
<span data-ttu-id="1ff5c-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1ff5c-119">Here is a JSON representation of the resource.</span></span>
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



