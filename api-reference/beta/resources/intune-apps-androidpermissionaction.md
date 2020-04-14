---
title: androidPermissionAction 资源类型
description: 在请求该权限时，Android 应用程序权限和适用于 Android 的操作之间的映射应采取的操作。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c0e1b793a447d29d1ed554e1b6466895ccc9e57f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459140"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="a64e5-103">androidPermissionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="a64e5-103">androidPermissionAction resource type</span></span>

<span data-ttu-id="a64e5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a64e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a64e5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a64e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a64e5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a64e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a64e5-107">在请求该权限时，Android 应用程序权限和适用于 Android 的操作之间的映射应采取的操作。</span><span class="sxs-lookup"><span data-stu-id="a64e5-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="a64e5-108">属性</span><span class="sxs-lookup"><span data-stu-id="a64e5-108">Properties</span></span>
|<span data-ttu-id="a64e5-109">属性</span><span class="sxs-lookup"><span data-stu-id="a64e5-109">Property</span></span>|<span data-ttu-id="a64e5-110">类型</span><span class="sxs-lookup"><span data-stu-id="a64e5-110">Type</span></span>|<span data-ttu-id="a64e5-111">说明</span><span class="sxs-lookup"><span data-stu-id="a64e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a64e5-112">拒绝</span><span class="sxs-lookup"><span data-stu-id="a64e5-112">permission</span></span>|<span data-ttu-id="a64e5-113">String</span><span class="sxs-lookup"><span data-stu-id="a64e5-113">String</span></span>|<span data-ttu-id="a64e5-114">Android 权限字符串，在官方 Android 文档中定义。</span><span class="sxs-lookup"><span data-stu-id="a64e5-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="a64e5-115">示例 "android. READ_CONTACTS"。</span><span class="sxs-lookup"><span data-stu-id="a64e5-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="a64e5-116">action</span><span class="sxs-lookup"><span data-stu-id="a64e5-116">action</span></span>|[<span data-ttu-id="a64e5-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="a64e5-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="a64e5-118">Android 权限操作的类型。</span><span class="sxs-lookup"><span data-stu-id="a64e5-118">Type of Android permission action.</span></span> <span data-ttu-id="a64e5-119">可取值为：`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="a64e5-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a64e5-120">关系</span><span class="sxs-lookup"><span data-stu-id="a64e5-120">Relationships</span></span>
<span data-ttu-id="a64e5-121">无</span><span class="sxs-lookup"><span data-stu-id="a64e5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a64e5-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a64e5-122">JSON Representation</span></span>
<span data-ttu-id="a64e5-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a64e5-123">Here is a JSON representation of the resource.</span></span>
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



