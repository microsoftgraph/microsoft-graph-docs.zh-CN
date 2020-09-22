---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b106811c802571edfd4da28134ea99883869c129
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030463"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="1c3ae-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="1c3ae-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="1c3ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1c3ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1c3ae-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1c3ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c3ae-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1c3ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c3ae-107">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="1c3ae-107">The identifier for an iOS app.</span></span>


<span data-ttu-id="1c3ae-108">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="1c3ae-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1c3ae-109">属性</span><span class="sxs-lookup"><span data-stu-id="1c3ae-109">Properties</span></span>
|<span data-ttu-id="1c3ae-110">属性</span><span class="sxs-lookup"><span data-stu-id="1c3ae-110">Property</span></span>|<span data-ttu-id="1c3ae-111">类型</span><span class="sxs-lookup"><span data-stu-id="1c3ae-111">Type</span></span>|<span data-ttu-id="1c3ae-112">说明</span><span class="sxs-lookup"><span data-stu-id="1c3ae-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c3ae-113">bundleId</span><span class="sxs-lookup"><span data-stu-id="1c3ae-113">bundleId</span></span>|<span data-ttu-id="1c3ae-114">String</span><span class="sxs-lookup"><span data-stu-id="1c3ae-114">String</span></span>|<span data-ttu-id="1c3ae-115">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="1c3ae-115">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c3ae-116">关系</span><span class="sxs-lookup"><span data-stu-id="1c3ae-116">Relationships</span></span>
<span data-ttu-id="1c3ae-117">无</span><span class="sxs-lookup"><span data-stu-id="1c3ae-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c3ae-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1c3ae-118">JSON Representation</span></span>
<span data-ttu-id="1c3ae-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c3ae-119">Here is a JSON representation of the resource.</span></span>
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






