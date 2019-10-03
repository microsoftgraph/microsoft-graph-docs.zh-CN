---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c43b559f1c1994d34ae0d4202b4970227d029df7
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366739"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="7f762-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f762-103">appListItem resource type</span></span>

> <span data-ttu-id="7f762-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f762-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f762-105">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="7f762-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="7f762-106">属性</span><span class="sxs-lookup"><span data-stu-id="7f762-106">Properties</span></span>
|<span data-ttu-id="7f762-107">属性</span><span class="sxs-lookup"><span data-stu-id="7f762-107">Property</span></span>|<span data-ttu-id="7f762-108">类型</span><span class="sxs-lookup"><span data-stu-id="7f762-108">Type</span></span>|<span data-ttu-id="7f762-109">说明</span><span class="sxs-lookup"><span data-stu-id="7f762-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f762-110">name</span><span class="sxs-lookup"><span data-stu-id="7f762-110">name</span></span>|<span data-ttu-id="7f762-111">字符串</span><span class="sxs-lookup"><span data-stu-id="7f762-111">String</span></span>|<span data-ttu-id="7f762-112">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="7f762-112">The application name</span></span>|
|<span data-ttu-id="7f762-113">publisher</span><span class="sxs-lookup"><span data-stu-id="7f762-113">publisher</span></span>|<span data-ttu-id="7f762-114">String</span><span class="sxs-lookup"><span data-stu-id="7f762-114">String</span></span>|<span data-ttu-id="7f762-115">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="7f762-115">The publisher of the application</span></span>|
|<span data-ttu-id="7f762-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7f762-116">appStoreUrl</span></span>|<span data-ttu-id="7f762-117">String</span><span class="sxs-lookup"><span data-stu-id="7f762-117">String</span></span>|<span data-ttu-id="7f762-118">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="7f762-118">The Store URL of the application</span></span>|
|<span data-ttu-id="7f762-119">appId</span><span class="sxs-lookup"><span data-stu-id="7f762-119">appId</span></span>|<span data-ttu-id="7f762-120">String</span><span class="sxs-lookup"><span data-stu-id="7f762-120">String</span></span>|<span data-ttu-id="7f762-121">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="7f762-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f762-122">关系</span><span class="sxs-lookup"><span data-stu-id="7f762-122">Relationships</span></span>
<span data-ttu-id="7f762-123">无</span><span class="sxs-lookup"><span data-stu-id="7f762-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f762-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f762-124">JSON Representation</span></span>
<span data-ttu-id="7f762-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f762-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```




