---
title: androidPermissionAction 资源类型
description: 在请求该权限时, Android 应用程序权限和适用于 Android 的操作之间的映射应采取的操作。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0d2aa07ae9064a6e7d04ea7e2f0dc07e06cfb627
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366887"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="13dc1-103">androidPermissionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="13dc1-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="13dc1-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13dc1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13dc1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13dc1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13dc1-106">在请求该权限时, Android 应用程序权限和适用于 Android 的操作之间的映射应采取的操作。</span><span class="sxs-lookup"><span data-stu-id="13dc1-106">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="13dc1-107">属性</span><span class="sxs-lookup"><span data-stu-id="13dc1-107">Properties</span></span>
|<span data-ttu-id="13dc1-108">属性</span><span class="sxs-lookup"><span data-stu-id="13dc1-108">Property</span></span>|<span data-ttu-id="13dc1-109">类型</span><span class="sxs-lookup"><span data-stu-id="13dc1-109">Type</span></span>|<span data-ttu-id="13dc1-110">说明</span><span class="sxs-lookup"><span data-stu-id="13dc1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13dc1-111">拒绝</span><span class="sxs-lookup"><span data-stu-id="13dc1-111">permission</span></span>|<span data-ttu-id="13dc1-112">String</span><span class="sxs-lookup"><span data-stu-id="13dc1-112">String</span></span>|<span data-ttu-id="13dc1-113">Android 权限字符串, 在官方 Android 文档中定义。</span><span class="sxs-lookup"><span data-stu-id="13dc1-113">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="13dc1-114">示例 "READ_CONTACTS"。</span><span class="sxs-lookup"><span data-stu-id="13dc1-114">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="13dc1-115">action</span><span class="sxs-lookup"><span data-stu-id="13dc1-115">action</span></span>|[<span data-ttu-id="13dc1-116">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="13dc1-116">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="13dc1-117">Android 权限操作的类型。</span><span class="sxs-lookup"><span data-stu-id="13dc1-117">Type of Android permission action.</span></span> <span data-ttu-id="13dc1-118">可取值为：`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="13dc1-118">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13dc1-119">关系</span><span class="sxs-lookup"><span data-stu-id="13dc1-119">Relationships</span></span>
<span data-ttu-id="13dc1-120">无</span><span class="sxs-lookup"><span data-stu-id="13dc1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13dc1-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13dc1-121">JSON Representation</span></span>
<span data-ttu-id="13dc1-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13dc1-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```



