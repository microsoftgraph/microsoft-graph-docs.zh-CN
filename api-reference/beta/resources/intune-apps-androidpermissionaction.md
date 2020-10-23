---
title: androidPermissionAction 资源类型
description: 在请求该权限时，Android 应用程序权限和适用于 Android 的操作之间的映射应采取的操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3c6e585a5a889a3af3b09f84f8a41c1fce2280c1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727552"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="dd32c-103">androidPermissionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd32c-103">androidPermissionAction resource type</span></span>

<span data-ttu-id="dd32c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd32c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd32c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dd32c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd32c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd32c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd32c-107">在请求该权限时，Android 应用程序权限和适用于 Android 的操作之间的映射应采取的操作。</span><span class="sxs-lookup"><span data-stu-id="dd32c-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="dd32c-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd32c-108">Properties</span></span>
|<span data-ttu-id="dd32c-109">属性</span><span class="sxs-lookup"><span data-stu-id="dd32c-109">Property</span></span>|<span data-ttu-id="dd32c-110">类型</span><span class="sxs-lookup"><span data-stu-id="dd32c-110">Type</span></span>|<span data-ttu-id="dd32c-111">说明</span><span class="sxs-lookup"><span data-stu-id="dd32c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd32c-112">拒绝</span><span class="sxs-lookup"><span data-stu-id="dd32c-112">permission</span></span>|<span data-ttu-id="dd32c-113">String</span><span class="sxs-lookup"><span data-stu-id="dd32c-113">String</span></span>|<span data-ttu-id="dd32c-114">Android 权限字符串，在官方 Android 文档中定义。</span><span class="sxs-lookup"><span data-stu-id="dd32c-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="dd32c-115">示例 "android.permission.READ_CONTACTS"。</span><span class="sxs-lookup"><span data-stu-id="dd32c-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="dd32c-116">action</span><span class="sxs-lookup"><span data-stu-id="dd32c-116">action</span></span>|[<span data-ttu-id="dd32c-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="dd32c-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="dd32c-118">Android 权限操作的类型。</span><span class="sxs-lookup"><span data-stu-id="dd32c-118">Type of Android permission action.</span></span> <span data-ttu-id="dd32c-119">可取值为：`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="dd32c-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd32c-120">关系</span><span class="sxs-lookup"><span data-stu-id="dd32c-120">Relationships</span></span>
<span data-ttu-id="dd32c-121">无</span><span class="sxs-lookup"><span data-stu-id="dd32c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd32c-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd32c-122">JSON Representation</span></span>
<span data-ttu-id="dd32c-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd32c-123">Here is a JSON representation of the resource.</span></span>
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





