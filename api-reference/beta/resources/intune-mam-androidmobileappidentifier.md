---
title: androidMobileAppIdentifier 资源类型
description: Android 应用的标识符。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8106475817a333838a9f7e6a591f15ddd2ce111d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563985"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="753b6-103">androidMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="753b6-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="753b6-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="753b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="753b6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="753b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="753b6-106">Android 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="753b6-106">The identifier for an Android app.</span></span>


<span data-ttu-id="753b6-107">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="753b6-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="753b6-108">属性</span><span class="sxs-lookup"><span data-stu-id="753b6-108">Properties</span></span>
|<span data-ttu-id="753b6-109">属性</span><span class="sxs-lookup"><span data-stu-id="753b6-109">Property</span></span>|<span data-ttu-id="753b6-110">类型</span><span class="sxs-lookup"><span data-stu-id="753b6-110">Type</span></span>|<span data-ttu-id="753b6-111">说明</span><span class="sxs-lookup"><span data-stu-id="753b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="753b6-112">packageId</span><span class="sxs-lookup"><span data-stu-id="753b6-112">packageId</span></span>|<span data-ttu-id="753b6-113">String</span><span class="sxs-lookup"><span data-stu-id="753b6-113">String</span></span>|<span data-ttu-id="753b6-114">应用的标识符，如 Play 商店中指定。</span><span class="sxs-lookup"><span data-stu-id="753b6-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="753b6-115">关系</span><span class="sxs-lookup"><span data-stu-id="753b6-115">Relationships</span></span>
<span data-ttu-id="753b6-116">无</span><span class="sxs-lookup"><span data-stu-id="753b6-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="753b6-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="753b6-117">JSON Representation</span></span>
<span data-ttu-id="753b6-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="753b6-118">Here is a JSON representation of the resource.</span></span>
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





