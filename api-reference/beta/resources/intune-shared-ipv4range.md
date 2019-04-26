---
title: iPv4Range 资源类型
description: IPv4 范围定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c896eb6f9a35992d7370cf29124d8072c171eb30
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550593"
---
# <a name="ipv4range-resource-type"></a><span data-ttu-id="113e2-103">iPv4Range 资源类型</span><span class="sxs-lookup"><span data-stu-id="113e2-103">iPv4Range resource type</span></span>

> <span data-ttu-id="113e2-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="113e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="113e2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="113e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="113e2-106">IPv4 范围定义。</span><span class="sxs-lookup"><span data-stu-id="113e2-106">IPv4 Range definition.</span></span>


<span data-ttu-id="113e2-107">继承自 [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="113e2-107">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="113e2-108">属性</span><span class="sxs-lookup"><span data-stu-id="113e2-108">Properties</span></span>
|<span data-ttu-id="113e2-109">属性</span><span class="sxs-lookup"><span data-stu-id="113e2-109">Property</span></span>|<span data-ttu-id="113e2-110">类型</span><span class="sxs-lookup"><span data-stu-id="113e2-110">Type</span></span>|<span data-ttu-id="113e2-111">说明</span><span class="sxs-lookup"><span data-stu-id="113e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="113e2-112">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="113e2-112">lowerAddress</span></span>|<span data-ttu-id="113e2-113">String</span><span class="sxs-lookup"><span data-stu-id="113e2-113">String</span></span>|<span data-ttu-id="113e2-114">较低的地址。</span><span class="sxs-lookup"><span data-stu-id="113e2-114">Lower address.</span></span>|
|<span data-ttu-id="113e2-115">upperAddress</span><span class="sxs-lookup"><span data-stu-id="113e2-115">upperAddress</span></span>|<span data-ttu-id="113e2-116">String</span><span class="sxs-lookup"><span data-stu-id="113e2-116">String</span></span>|<span data-ttu-id="113e2-117">地址上限。</span><span class="sxs-lookup"><span data-stu-id="113e2-117">Upper address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="113e2-118">关系</span><span class="sxs-lookup"><span data-stu-id="113e2-118">Relationships</span></span>
<span data-ttu-id="113e2-119">无</span><span class="sxs-lookup"><span data-stu-id="113e2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="113e2-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="113e2-120">JSON Representation</span></span>
<span data-ttu-id="113e2-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="113e2-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iPv4Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv4Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```





