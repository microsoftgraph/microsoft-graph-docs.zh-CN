---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b485d5b0ba526971a29e98d764aa459e870fd725
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533205"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="49298-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="49298-103">iosMobileAppIdentifier resource type</span></span>

<span data-ttu-id="49298-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49298-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49298-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49298-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49298-106">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="49298-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="49298-107">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="49298-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="49298-108">属性</span><span class="sxs-lookup"><span data-stu-id="49298-108">Properties</span></span>
|<span data-ttu-id="49298-109">属性</span><span class="sxs-lookup"><span data-stu-id="49298-109">Property</span></span>|<span data-ttu-id="49298-110">类型</span><span class="sxs-lookup"><span data-stu-id="49298-110">Type</span></span>|<span data-ttu-id="49298-111">说明</span><span class="sxs-lookup"><span data-stu-id="49298-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49298-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="49298-112">bundleId</span></span>|<span data-ttu-id="49298-113">String</span><span class="sxs-lookup"><span data-stu-id="49298-113">String</span></span>|<span data-ttu-id="49298-114">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="49298-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49298-115">关系</span><span class="sxs-lookup"><span data-stu-id="49298-115">Relationships</span></span>
<span data-ttu-id="49298-116">无</span><span class="sxs-lookup"><span data-stu-id="49298-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49298-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49298-117">JSON Representation</span></span>
<span data-ttu-id="49298-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49298-118">Here is a JSON representation of the resource.</span></span>
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




