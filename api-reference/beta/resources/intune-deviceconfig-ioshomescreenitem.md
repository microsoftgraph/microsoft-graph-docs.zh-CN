---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b4685c62177dcb7d8cdf0f827d5af085d571d9b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521612"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="1d0fb-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d0fb-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="1d0fb-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1d0fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d0fb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1d0fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d0fb-106">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="1d0fb-106">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="1d0fb-107">属性</span><span class="sxs-lookup"><span data-stu-id="1d0fb-107">Properties</span></span>
|<span data-ttu-id="1d0fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="1d0fb-108">Property</span></span>|<span data-ttu-id="1d0fb-109">类型</span><span class="sxs-lookup"><span data-stu-id="1d0fb-109">Type</span></span>|<span data-ttu-id="1d0fb-110">说明</span><span class="sxs-lookup"><span data-stu-id="1d0fb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d0fb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1d0fb-111">displayName</span></span>|<span data-ttu-id="1d0fb-112">String</span><span class="sxs-lookup"><span data-stu-id="1d0fb-112">String</span></span>|<span data-ttu-id="1d0fb-113">应用的名称</span><span class="sxs-lookup"><span data-stu-id="1d0fb-113">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d0fb-114">关系</span><span class="sxs-lookup"><span data-stu-id="1d0fb-114">Relationships</span></span>
<span data-ttu-id="1d0fb-115">无</span><span class="sxs-lookup"><span data-stu-id="1d0fb-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d0fb-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d0fb-116">JSON Representation</span></span>
<span data-ttu-id="1d0fb-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d0fb-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```





