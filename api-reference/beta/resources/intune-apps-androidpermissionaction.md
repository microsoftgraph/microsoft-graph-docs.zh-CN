---
title: androidPermissionAction 资源类型
description: 在请求该权限时，Android 应用程序权限和适用于 Android 的操作之间的映射应采取的操作。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52b105c831399b935196254d794bd5da513d19f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42494098"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="efa44-103">androidPermissionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="efa44-103">androidPermissionAction resource type</span></span>

<span data-ttu-id="efa44-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="efa44-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efa44-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="efa44-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efa44-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="efa44-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efa44-107">在请求该权限时，Android 应用程序权限和适用于 Android 的操作之间的映射应采取的操作。</span><span class="sxs-lookup"><span data-stu-id="efa44-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="efa44-108">属性</span><span class="sxs-lookup"><span data-stu-id="efa44-108">Properties</span></span>
|<span data-ttu-id="efa44-109">属性</span><span class="sxs-lookup"><span data-stu-id="efa44-109">Property</span></span>|<span data-ttu-id="efa44-110">类型</span><span class="sxs-lookup"><span data-stu-id="efa44-110">Type</span></span>|<span data-ttu-id="efa44-111">说明</span><span class="sxs-lookup"><span data-stu-id="efa44-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efa44-112">拒绝</span><span class="sxs-lookup"><span data-stu-id="efa44-112">permission</span></span>|<span data-ttu-id="efa44-113">String</span><span class="sxs-lookup"><span data-stu-id="efa44-113">String</span></span>|<span data-ttu-id="efa44-114">Android 权限字符串，在官方 Android 文档中定义。</span><span class="sxs-lookup"><span data-stu-id="efa44-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="efa44-115">示例 "android. READ_CONTACTS"。</span><span class="sxs-lookup"><span data-stu-id="efa44-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="efa44-116">action</span><span class="sxs-lookup"><span data-stu-id="efa44-116">action</span></span>|[<span data-ttu-id="efa44-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="efa44-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="efa44-118">Android 权限操作的类型。</span><span class="sxs-lookup"><span data-stu-id="efa44-118">Type of Android permission action.</span></span> <span data-ttu-id="efa44-119">可取值为：`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="efa44-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efa44-120">关系</span><span class="sxs-lookup"><span data-stu-id="efa44-120">Relationships</span></span>
<span data-ttu-id="efa44-121">无</span><span class="sxs-lookup"><span data-stu-id="efa44-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efa44-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efa44-122">JSON Representation</span></span>
<span data-ttu-id="efa44-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efa44-123">Here is a JSON representation of the resource.</span></span>
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



