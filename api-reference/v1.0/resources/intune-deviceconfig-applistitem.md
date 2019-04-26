---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb81c8edfae3f9b33be4636e9fd7f15fa758e789
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575091"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="93e28-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="93e28-103">appListItem resource type</span></span>

> <span data-ttu-id="93e28-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="93e28-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93e28-105">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="93e28-105">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="93e28-106">属性</span><span class="sxs-lookup"><span data-stu-id="93e28-106">Properties</span></span>
|<span data-ttu-id="93e28-107">属性</span><span class="sxs-lookup"><span data-stu-id="93e28-107">Property</span></span>|<span data-ttu-id="93e28-108">类型</span><span class="sxs-lookup"><span data-stu-id="93e28-108">Type</span></span>|<span data-ttu-id="93e28-109">说明</span><span class="sxs-lookup"><span data-stu-id="93e28-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93e28-110">name</span><span class="sxs-lookup"><span data-stu-id="93e28-110">name</span></span>|<span data-ttu-id="93e28-111">String</span><span class="sxs-lookup"><span data-stu-id="93e28-111">String</span></span>|<span data-ttu-id="93e28-112">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="93e28-112">The application name</span></span>|
|<span data-ttu-id="93e28-113">publisher</span><span class="sxs-lookup"><span data-stu-id="93e28-113">publisher</span></span>|<span data-ttu-id="93e28-114">String</span><span class="sxs-lookup"><span data-stu-id="93e28-114">String</span></span>|<span data-ttu-id="93e28-115">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="93e28-115">The publisher of the application</span></span>|
|<span data-ttu-id="93e28-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="93e28-116">appStoreUrl</span></span>|<span data-ttu-id="93e28-117">String</span><span class="sxs-lookup"><span data-stu-id="93e28-117">String</span></span>|<span data-ttu-id="93e28-118">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="93e28-118">The Store URL of the application</span></span>|
|<span data-ttu-id="93e28-119">appId</span><span class="sxs-lookup"><span data-stu-id="93e28-119">appId</span></span>|<span data-ttu-id="93e28-120">String</span><span class="sxs-lookup"><span data-stu-id="93e28-120">String</span></span>|<span data-ttu-id="93e28-121">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="93e28-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="93e28-122">关系</span><span class="sxs-lookup"><span data-stu-id="93e28-122">Relationships</span></span>
<span data-ttu-id="93e28-123">无</span><span class="sxs-lookup"><span data-stu-id="93e28-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93e28-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="93e28-124">JSON Representation</span></span>
<span data-ttu-id="93e28-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93e28-125">Here is a JSON representation of the resource.</span></span>
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



