---
title: androidMobileAppIdentifier 资源类型
description: Android 应用的标识符。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6c26c41ffcb36ee325f5e0fae907916a418fb8b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410278"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="c838f-103">androidMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="c838f-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="c838f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c838f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c838f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c838f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c838f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c838f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c838f-107">Android 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="c838f-107">The identifier for an Android app.</span></span>


<span data-ttu-id="c838f-108">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="c838f-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c838f-109">属性</span><span class="sxs-lookup"><span data-stu-id="c838f-109">Properties</span></span>
|<span data-ttu-id="c838f-110">属性</span><span class="sxs-lookup"><span data-stu-id="c838f-110">Property</span></span>|<span data-ttu-id="c838f-111">类型</span><span class="sxs-lookup"><span data-stu-id="c838f-111">Type</span></span>|<span data-ttu-id="c838f-112">说明</span><span class="sxs-lookup"><span data-stu-id="c838f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c838f-113">packageId</span><span class="sxs-lookup"><span data-stu-id="c838f-113">packageId</span></span>|<span data-ttu-id="c838f-114">String</span><span class="sxs-lookup"><span data-stu-id="c838f-114">String</span></span>|<span data-ttu-id="c838f-115">应用的标识符，如 Play 商店中指定。</span><span class="sxs-lookup"><span data-stu-id="c838f-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c838f-116">关系</span><span class="sxs-lookup"><span data-stu-id="c838f-116">Relationships</span></span>
<span data-ttu-id="c838f-117">无</span><span class="sxs-lookup"><span data-stu-id="c838f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c838f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c838f-118">JSON Representation</span></span>
<span data-ttu-id="c838f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c838f-119">Here is a JSON representation of the resource.</span></span>
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




