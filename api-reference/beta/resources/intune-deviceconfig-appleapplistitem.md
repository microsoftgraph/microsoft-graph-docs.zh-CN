---
title: appleAppListItem 资源类型
description: 表示托管 Apple 应用程序列表中的应用程序
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a95905ef8076883ebdeea4a5ea6973017e511fee
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283747"
---
# <a name="appleapplistitem-resource-type"></a><span data-ttu-id="a9fe0-103">appleAppListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9fe0-103">appleAppListItem resource type</span></span>

<span data-ttu-id="a9fe0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9fe0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9fe0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9fe0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9fe0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9fe0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9fe0-107">表示托管 Apple 应用程序列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="a9fe0-107">Represents an app in the list of managed Apple applications</span></span>


<span data-ttu-id="a9fe0-108">继承自 [appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="a9fe0-108">Inherits from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a9fe0-109">属性</span><span class="sxs-lookup"><span data-stu-id="a9fe0-109">Properties</span></span>
|<span data-ttu-id="a9fe0-110">属性</span><span class="sxs-lookup"><span data-stu-id="a9fe0-110">Property</span></span>|<span data-ttu-id="a9fe0-111">类型</span><span class="sxs-lookup"><span data-stu-id="a9fe0-111">Type</span></span>|<span data-ttu-id="a9fe0-112">Description</span><span class="sxs-lookup"><span data-stu-id="a9fe0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9fe0-113">name</span><span class="sxs-lookup"><span data-stu-id="a9fe0-113">name</span></span>|<span data-ttu-id="a9fe0-114">字符串</span><span class="sxs-lookup"><span data-stu-id="a9fe0-114">String</span></span>|<span data-ttu-id="a9fe0-115">从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序名称</span><span class="sxs-lookup"><span data-stu-id="a9fe0-115">The application name Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="a9fe0-116">发布者</span><span class="sxs-lookup"><span data-stu-id="a9fe0-116">publisher</span></span>|<span data-ttu-id="a9fe0-117">String</span><span class="sxs-lookup"><span data-stu-id="a9fe0-117">String</span></span>|<span data-ttu-id="a9fe0-118">从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序的发布者</span><span class="sxs-lookup"><span data-stu-id="a9fe0-118">The publisher of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="a9fe0-119">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a9fe0-119">appStoreUrl</span></span>|<span data-ttu-id="a9fe0-120">String</span><span class="sxs-lookup"><span data-stu-id="a9fe0-120">String</span></span>|<span data-ttu-id="a9fe0-121">继承自[appListItem](../resources/intune-deviceconfig-applistitem.md)的应用程序的存储 URL</span><span class="sxs-lookup"><span data-stu-id="a9fe0-121">The Store URL of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="a9fe0-122">appId</span><span class="sxs-lookup"><span data-stu-id="a9fe0-122">appId</span></span>|<span data-ttu-id="a9fe0-123">String</span><span class="sxs-lookup"><span data-stu-id="a9fe0-123">String</span></span>|<span data-ttu-id="a9fe0-124">从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序的应用程序或捆绑包标识符</span><span class="sxs-lookup"><span data-stu-id="a9fe0-124">The application or bundle identifier of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9fe0-125">关系</span><span class="sxs-lookup"><span data-stu-id="a9fe0-125">Relationships</span></span>
<span data-ttu-id="a9fe0-126">无</span><span class="sxs-lookup"><span data-stu-id="a9fe0-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9fe0-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9fe0-127">JSON Representation</span></span>
<span data-ttu-id="a9fe0-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9fe0-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleAppListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleAppListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```




