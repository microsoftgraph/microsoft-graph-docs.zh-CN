---
title: androidMobileAppIdentifier 资源类型
description: Android 应用的标识符。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 07dcc1bd7480439f5c1dd71afa36e18a5df0eb14
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754530"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="b4f1f-103">androidMobileAppIdentifier 资源类型</span><span class="sxs-lookup"><span data-stu-id="b4f1f-103">androidMobileAppIdentifier resource type</span></span>

<span data-ttu-id="b4f1f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4f1f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4f1f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4f1f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4f1f-106">Android 应用的标识符。</span><span class="sxs-lookup"><span data-stu-id="b4f1f-106">The identifier for an Android app.</span></span>


<span data-ttu-id="b4f1f-107">继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="b4f1f-107">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b4f1f-108">属性</span><span class="sxs-lookup"><span data-stu-id="b4f1f-108">Properties</span></span>
|<span data-ttu-id="b4f1f-109">属性</span><span class="sxs-lookup"><span data-stu-id="b4f1f-109">Property</span></span>|<span data-ttu-id="b4f1f-110">类型</span><span class="sxs-lookup"><span data-stu-id="b4f1f-110">Type</span></span>|<span data-ttu-id="b4f1f-111">Description</span><span class="sxs-lookup"><span data-stu-id="b4f1f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4f1f-112">packageId</span><span class="sxs-lookup"><span data-stu-id="b4f1f-112">packageId</span></span>|<span data-ttu-id="b4f1f-113">String</span><span class="sxs-lookup"><span data-stu-id="b4f1f-113">String</span></span>|<span data-ttu-id="b4f1f-114">应用的标识符，如 Play 商店中指定。</span><span class="sxs-lookup"><span data-stu-id="b4f1f-114">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4f1f-115">关系</span><span class="sxs-lookup"><span data-stu-id="b4f1f-115">Relationships</span></span>
<span data-ttu-id="b4f1f-116">无</span><span class="sxs-lookup"><span data-stu-id="b4f1f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4f1f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b4f1f-117">JSON Representation</span></span>
<span data-ttu-id="b4f1f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b4f1f-118">Here is a JSON representation of the resource.</span></span>
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




