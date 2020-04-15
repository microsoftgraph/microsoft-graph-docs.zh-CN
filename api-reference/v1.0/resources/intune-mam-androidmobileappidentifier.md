---
title: androidMobileAppIdentifier 资源类型
description: Android 应用的标识符。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b610cbfa4ba7296a9b8427b9bb49f7b4493f773
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474122"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="7ced1-103">androidMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ced1-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="7ced1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ced1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ced1-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ced1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ced1-106">Android 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="7ced1-106">The identifier for an Android app.</span></span>


<span data-ttu-id="7ced1-107">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="7ced1-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7ced1-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ced1-108">Properties</span></span>
|<span data-ttu-id="7ced1-109">属性</span><span class="sxs-lookup"><span data-stu-id="7ced1-109">Property</span></span>|<span data-ttu-id="7ced1-110">类型</span><span class="sxs-lookup"><span data-stu-id="7ced1-110">Type</span></span>|<span data-ttu-id="7ced1-111">说明</span><span class="sxs-lookup"><span data-stu-id="7ced1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ced1-112">packageId</span><span class="sxs-lookup"><span data-stu-id="7ced1-112">packageId</span></span>|<span data-ttu-id="7ced1-113">String</span><span class="sxs-lookup"><span data-stu-id="7ced1-113">String</span></span>|<span data-ttu-id="7ced1-114">应用的标识符，如 Play 商店中指定。</span><span class="sxs-lookup"><span data-stu-id="7ced1-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ced1-115">关系</span><span class="sxs-lookup"><span data-stu-id="7ced1-115">Relationships</span></span>
<span data-ttu-id="7ced1-116">无</span><span class="sxs-lookup"><span data-stu-id="7ced1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ced1-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ced1-117">JSON Representation</span></span>
<span data-ttu-id="7ced1-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ced1-118">Here is a JSON representation of the resource.</span></span>
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







