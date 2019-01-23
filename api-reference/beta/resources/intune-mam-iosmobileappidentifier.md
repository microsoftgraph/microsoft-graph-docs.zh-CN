---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ddd09f6d1f0d49b00282c55bfa6dcbef1fcb1d2c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409928"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="2c3ef-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="2c3ef-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="2c3ef-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2c3ef-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2c3ef-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2c3ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c3ef-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2c3ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c3ef-107">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="2c3ef-107">The identifier for an iOS app.</span></span>


<span data-ttu-id="2c3ef-108">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="2c3ef-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2c3ef-109">属性</span><span class="sxs-lookup"><span data-stu-id="2c3ef-109">Properties</span></span>
|<span data-ttu-id="2c3ef-110">属性</span><span class="sxs-lookup"><span data-stu-id="2c3ef-110">Property</span></span>|<span data-ttu-id="2c3ef-111">类型</span><span class="sxs-lookup"><span data-stu-id="2c3ef-111">Type</span></span>|<span data-ttu-id="2c3ef-112">说明</span><span class="sxs-lookup"><span data-stu-id="2c3ef-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c3ef-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="2c3ef-113">bundleId</span></span>|<span data-ttu-id="2c3ef-114">String</span><span class="sxs-lookup"><span data-stu-id="2c3ef-114">String</span></span>|<span data-ttu-id="2c3ef-115">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="2c3ef-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c3ef-116">关系</span><span class="sxs-lookup"><span data-stu-id="2c3ef-116">Relationships</span></span>
<span data-ttu-id="2c3ef-117">无</span><span class="sxs-lookup"><span data-stu-id="2c3ef-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c3ef-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2c3ef-118">JSON Representation</span></span>
<span data-ttu-id="2c3ef-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2c3ef-119">Here is a JSON representation of the resource.</span></span>
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




