---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 690703b5355a20a609363cc7c0ffd7a4574b903f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010880"
---
# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="60323-103">iosMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="60323-103">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="60323-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="60323-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60323-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="60323-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60323-106">iOS 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="60323-106">The identifier for an iOS app.</span></span>


<span data-ttu-id="60323-107">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="60323-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="60323-108">属性</span><span class="sxs-lookup"><span data-stu-id="60323-108">Properties</span></span>
|<span data-ttu-id="60323-109">属性</span><span class="sxs-lookup"><span data-stu-id="60323-109">Property</span></span>|<span data-ttu-id="60323-110">类型</span><span class="sxs-lookup"><span data-stu-id="60323-110">Type</span></span>|<span data-ttu-id="60323-111">说明</span><span class="sxs-lookup"><span data-stu-id="60323-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60323-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="60323-112">bundleId</span></span>|<span data-ttu-id="60323-113">String</span><span class="sxs-lookup"><span data-stu-id="60323-113">String</span></span>|<span data-ttu-id="60323-114">应用的标识符，如应用商店中指定。</span><span class="sxs-lookup"><span data-stu-id="60323-114">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60323-115">关系</span><span class="sxs-lookup"><span data-stu-id="60323-115">Relationships</span></span>
<span data-ttu-id="60323-116">无</span><span class="sxs-lookup"><span data-stu-id="60323-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60323-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60323-117">JSON Representation</span></span>
<span data-ttu-id="60323-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60323-118">Here is a JSON representation of the resource.</span></span>
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





