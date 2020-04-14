---
title: iosWebContentFilterSpecificWebsitesAccess 资源类型
description: 表示 iOS Web 内容筛选器设置类型，该类型将 URL 书签安装到 iOS 内置浏览器中。 在课堂中，教师希望学生通过在其 iOS 设备上配置的浏览器书签来导航网站，而不能访问其他网站，这是一个示例方案。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f6e68fecd5bed0f51f89d15714ac3f2c95516396
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43440038"
---
# <a name="ioswebcontentfilterspecificwebsitesaccess-resource-type"></a><span data-ttu-id="6a26a-104">iosWebContentFilterSpecificWebsitesAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a26a-104">iosWebContentFilterSpecificWebsitesAccess resource type</span></span>

<span data-ttu-id="6a26a-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a26a-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a26a-106">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6a26a-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a26a-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a26a-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a26a-108">表示 iOS Web 内容筛选器设置类型，该类型将 URL 书签安装到 iOS 内置浏览器中。</span><span class="sxs-lookup"><span data-stu-id="6a26a-108">Represents an iOS Web Content Filter setting type, which installs URL bookmarks into iOS built-in browser.</span></span> <span data-ttu-id="6a26a-109">在课堂中，教师希望学生通过在其 iOS 设备上配置的浏览器书签来导航网站，而不能访问其他网站，这是一个示例方案。</span><span class="sxs-lookup"><span data-stu-id="6a26a-109">An example scenario is in the classroom where teachers would like the students to navigate websites through browser bookmarks configured on their iOS devices, and no access to other sites.</span></span>


<span data-ttu-id="6a26a-110">继承自[iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="6a26a-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6a26a-111">属性</span><span class="sxs-lookup"><span data-stu-id="6a26a-111">Properties</span></span>
|<span data-ttu-id="6a26a-112">属性</span><span class="sxs-lookup"><span data-stu-id="6a26a-112">Property</span></span>|<span data-ttu-id="6a26a-113">类型</span><span class="sxs-lookup"><span data-stu-id="6a26a-113">Type</span></span>|<span data-ttu-id="6a26a-114">说明</span><span class="sxs-lookup"><span data-stu-id="6a26a-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a26a-115">specificWebsitesOnly</span><span class="sxs-lookup"><span data-stu-id="6a26a-115">specificWebsitesOnly</span></span>|<span data-ttu-id="6a26a-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)集合</span><span class="sxs-lookup"><span data-stu-id="6a26a-116">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="6a26a-117">将安装到内置浏览器和用户的 URL 书签仅允许通过书签访问网站。</span><span class="sxs-lookup"><span data-stu-id="6a26a-117">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="6a26a-118">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6a26a-118">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6a26a-119">websiteList</span><span class="sxs-lookup"><span data-stu-id="6a26a-119">websiteList</span></span>|<span data-ttu-id="6a26a-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md)集合</span><span class="sxs-lookup"><span data-stu-id="6a26a-120">[iosBookmark](../resources/intune-deviceconfig-iosbookmark.md) collection</span></span>|<span data-ttu-id="6a26a-121">将安装到内置浏览器和用户的 URL 书签仅允许通过书签访问网站。</span><span class="sxs-lookup"><span data-stu-id="6a26a-121">URL bookmarks which will be installed into built-in browser and user is only allowed to access websites through bookmarks.</span></span> <span data-ttu-id="6a26a-122">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6a26a-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a26a-123">关系</span><span class="sxs-lookup"><span data-stu-id="6a26a-123">Relationships</span></span>
<span data-ttu-id="6a26a-124">无</span><span class="sxs-lookup"><span data-stu-id="6a26a-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a26a-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a26a-125">JSON Representation</span></span>
<span data-ttu-id="6a26a-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a26a-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
  "specificWebsitesOnly": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ],
  "websiteList": [
    {
      "@odata.type": "microsoft.graph.iosBookmark",
      "url": "String",
      "bookmarkFolder": "String",
      "displayName": "String"
    }
  ]
}
```



