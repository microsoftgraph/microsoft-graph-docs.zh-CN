---
title: appListItem 资源类型
description: 表示托管应用程序列表中的应用
author: tfitzmac
ms.openlocfilehash: a7e33b986f95f610abff2c7b5321f48f3668e488
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323595"
---
# <a name="applistitem-resource-type"></a><span data-ttu-id="9796b-103">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="9796b-103">appListItem resource type</span></span>

> <span data-ttu-id="9796b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9796b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9796b-105">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="9796b-105">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="9796b-106">属性</span><span class="sxs-lookup"><span data-stu-id="9796b-106">Properties</span></span>
|<span data-ttu-id="9796b-107">属性</span><span class="sxs-lookup"><span data-stu-id="9796b-107">Property</span></span>|<span data-ttu-id="9796b-108">类型</span><span class="sxs-lookup"><span data-stu-id="9796b-108">Type</span></span>|<span data-ttu-id="9796b-109">说明</span><span class="sxs-lookup"><span data-stu-id="9796b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9796b-110">name</span><span class="sxs-lookup"><span data-stu-id="9796b-110">name</span></span>|<span data-ttu-id="9796b-111">String</span><span class="sxs-lookup"><span data-stu-id="9796b-111">String</span></span>|<span data-ttu-id="9796b-112">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="9796b-112">The application name</span></span>|
|<span data-ttu-id="9796b-113">publisher</span><span class="sxs-lookup"><span data-stu-id="9796b-113">publisher</span></span>|<span data-ttu-id="9796b-114">String</span><span class="sxs-lookup"><span data-stu-id="9796b-114">String</span></span>|<span data-ttu-id="9796b-115">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="9796b-115">The publisher of the application</span></span>|
|<span data-ttu-id="9796b-116">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="9796b-116">appStoreUrl</span></span>|<span data-ttu-id="9796b-117">String</span><span class="sxs-lookup"><span data-stu-id="9796b-117">String</span></span>|<span data-ttu-id="9796b-118">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="9796b-118">The Store URL of the application</span></span>|
|<span data-ttu-id="9796b-119">appId</span><span class="sxs-lookup"><span data-stu-id="9796b-119">appId</span></span>|<span data-ttu-id="9796b-120">String</span><span class="sxs-lookup"><span data-stu-id="9796b-120">String</span></span>|<span data-ttu-id="9796b-121">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="9796b-121">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="9796b-122">关系</span><span class="sxs-lookup"><span data-stu-id="9796b-122">Relationships</span></span>
<span data-ttu-id="9796b-123">无</span><span class="sxs-lookup"><span data-stu-id="9796b-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9796b-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9796b-124">JSON Representation</span></span>
<span data-ttu-id="9796b-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9796b-125">Here is a JSON representation of the resource.</span></span>
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



