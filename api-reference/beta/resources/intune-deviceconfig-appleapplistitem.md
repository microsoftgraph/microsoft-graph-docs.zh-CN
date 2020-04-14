---
title: appleAppListItem 资源类型
description: 表示托管 Apple 应用程序列表中的应用程序
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f4804f3834a63a3c446c09d383c2244def97398
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470123"
---
# <a name="appleapplistitem-resource-type"></a><span data-ttu-id="7072d-103">appleAppListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="7072d-103">appleAppListItem resource type</span></span>

<span data-ttu-id="7072d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7072d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7072d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7072d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7072d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7072d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7072d-107">表示托管 Apple 应用程序列表中的应用程序</span><span class="sxs-lookup"><span data-stu-id="7072d-107">Represents an app in the list of managed Apple applications</span></span>


<span data-ttu-id="7072d-108">继承自[appListItem](../resources/intune-deviceconfig-applistitem.md)</span><span class="sxs-lookup"><span data-stu-id="7072d-108">Inherits from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7072d-109">属性</span><span class="sxs-lookup"><span data-stu-id="7072d-109">Properties</span></span>
|<span data-ttu-id="7072d-110">属性</span><span class="sxs-lookup"><span data-stu-id="7072d-110">Property</span></span>|<span data-ttu-id="7072d-111">类型</span><span class="sxs-lookup"><span data-stu-id="7072d-111">Type</span></span>|<span data-ttu-id="7072d-112">说明</span><span class="sxs-lookup"><span data-stu-id="7072d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7072d-113">name</span><span class="sxs-lookup"><span data-stu-id="7072d-113">name</span></span>|<span data-ttu-id="7072d-114">字符串</span><span class="sxs-lookup"><span data-stu-id="7072d-114">String</span></span>|<span data-ttu-id="7072d-115">从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序名称</span><span class="sxs-lookup"><span data-stu-id="7072d-115">The application name Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="7072d-116">发布者</span><span class="sxs-lookup"><span data-stu-id="7072d-116">publisher</span></span>|<span data-ttu-id="7072d-117">String</span><span class="sxs-lookup"><span data-stu-id="7072d-117">String</span></span>|<span data-ttu-id="7072d-118">从[AppListItem](../resources/intune-deviceconfig-applistitem.md)继承的应用程序的发布者</span><span class="sxs-lookup"><span data-stu-id="7072d-118">The publisher of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="7072d-119">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7072d-119">appStoreUrl</span></span>|<span data-ttu-id="7072d-120">String</span><span class="sxs-lookup"><span data-stu-id="7072d-120">String</span></span>|<span data-ttu-id="7072d-121">继承自[appListItem](../resources/intune-deviceconfig-applistitem.md)的应用程序的存储 URL</span><span class="sxs-lookup"><span data-stu-id="7072d-121">The Store URL of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|
|<span data-ttu-id="7072d-122">appId</span><span class="sxs-lookup"><span data-stu-id="7072d-122">appId</span></span>|<span data-ttu-id="7072d-123">String</span><span class="sxs-lookup"><span data-stu-id="7072d-123">String</span></span>|<span data-ttu-id="7072d-124">继承自[appListItem](../resources/intune-deviceconfig-applistitem.md)的应用程序的捆绑包标识符</span><span class="sxs-lookup"><span data-stu-id="7072d-124">The bundle identifier of the application Inherited from [appListItem](../resources/intune-deviceconfig-applistitem.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7072d-125">关系</span><span class="sxs-lookup"><span data-stu-id="7072d-125">Relationships</span></span>
<span data-ttu-id="7072d-126">无</span><span class="sxs-lookup"><span data-stu-id="7072d-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7072d-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7072d-127">JSON Representation</span></span>
<span data-ttu-id="7072d-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7072d-128">Here is a JSON representation of the resource.</span></span>
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



