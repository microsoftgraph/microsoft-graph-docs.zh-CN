---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a018be94068c0edf478f78fc692b9abcd036a060
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449160"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="11862-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="11862-103">appListItem resource type</span></span>

<span data-ttu-id="11862-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11862-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11862-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11862-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11862-106">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="11862-106">Represents an app in the list of managed applications</span></span>

## <a name="properties"></a><span data-ttu-id="11862-107">属性</span><span class="sxs-lookup"><span data-stu-id="11862-107">Properties</span></span>
|<span data-ttu-id="11862-108">属性</span><span class="sxs-lookup"><span data-stu-id="11862-108">Property</span></span>|<span data-ttu-id="11862-109">类型</span><span class="sxs-lookup"><span data-stu-id="11862-109">Type</span></span>|<span data-ttu-id="11862-110">说明</span><span class="sxs-lookup"><span data-stu-id="11862-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11862-111">name</span><span class="sxs-lookup"><span data-stu-id="11862-111">name</span></span>|<span data-ttu-id="11862-112">字符串</span><span class="sxs-lookup"><span data-stu-id="11862-112">String</span></span>|<span data-ttu-id="11862-113">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="11862-113">The application name</span></span>|
|<span data-ttu-id="11862-114">publisher</span><span class="sxs-lookup"><span data-stu-id="11862-114">publisher</span></span>|<span data-ttu-id="11862-115">String</span><span class="sxs-lookup"><span data-stu-id="11862-115">String</span></span>|<span data-ttu-id="11862-116">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="11862-116">The publisher of the application</span></span>|
|<span data-ttu-id="11862-117">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="11862-117">appStoreUrl</span></span>|<span data-ttu-id="11862-118">String</span><span class="sxs-lookup"><span data-stu-id="11862-118">String</span></span>|<span data-ttu-id="11862-119">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="11862-119">The Store URL of the application</span></span>|
|<span data-ttu-id="11862-120">appId</span><span class="sxs-lookup"><span data-stu-id="11862-120">appId</span></span>|<span data-ttu-id="11862-121">String</span><span class="sxs-lookup"><span data-stu-id="11862-121">String</span></span>|<span data-ttu-id="11862-122">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="11862-122">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="11862-123">关系</span><span class="sxs-lookup"><span data-stu-id="11862-123">Relationships</span></span>
<span data-ttu-id="11862-124">无</span><span class="sxs-lookup"><span data-stu-id="11862-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11862-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11862-125">JSON Representation</span></span>
<span data-ttu-id="11862-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11862-126">Here is a JSON representation of the resource.</span></span>
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







