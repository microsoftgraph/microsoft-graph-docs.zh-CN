---
title: androidPermissionAction 资源类型
description: 请求的权限时，应采取 Android 应用程序权限和 Android 的操作之间的映射。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62355c3427083df09963e316f3b6b3c104a8662f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425629"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="bb1fe-103">androidPermissionAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb1fe-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="bb1fe-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="bb1fe-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bb1fe-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bb1fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb1fe-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb1fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb1fe-107">请求的权限时，应采取 Android 应用程序权限和 Android 的操作之间的映射。</span><span class="sxs-lookup"><span data-stu-id="bb1fe-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="bb1fe-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb1fe-108">Properties</span></span>
|<span data-ttu-id="bb1fe-109">属性</span><span class="sxs-lookup"><span data-stu-id="bb1fe-109">Property</span></span>|<span data-ttu-id="bb1fe-110">类型</span><span class="sxs-lookup"><span data-stu-id="bb1fe-110">Type</span></span>|<span data-ttu-id="bb1fe-111">说明</span><span class="sxs-lookup"><span data-stu-id="bb1fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb1fe-112">权限</span><span class="sxs-lookup"><span data-stu-id="bb1fe-112">permission</span></span>|<span data-ttu-id="bb1fe-113">String</span><span class="sxs-lookup"><span data-stu-id="bb1fe-113">String</span></span>|<span data-ttu-id="bb1fe-114">正式 Android 文档中定义的 android 权限字符串。</span><span class="sxs-lookup"><span data-stu-id="bb1fe-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="bb1fe-115">示例 android.permission.READ_CONTACTS。</span><span class="sxs-lookup"><span data-stu-id="bb1fe-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="bb1fe-116">action</span><span class="sxs-lookup"><span data-stu-id="bb1fe-116">action</span></span>|[<span data-ttu-id="bb1fe-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="bb1fe-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="bb1fe-118">Android 权限操作的类型。</span><span class="sxs-lookup"><span data-stu-id="bb1fe-118">Type of Android permission action.</span></span> <span data-ttu-id="bb1fe-119">可取值为：`prompt`、`autoGrant`、`autoDeny`。</span><span class="sxs-lookup"><span data-stu-id="bb1fe-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb1fe-120">Relationships</span><span class="sxs-lookup"><span data-stu-id="bb1fe-120">Relationships</span></span>
<span data-ttu-id="bb1fe-121">无</span><span class="sxs-lookup"><span data-stu-id="bb1fe-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb1fe-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb1fe-122">JSON Representation</span></span>
<span data-ttu-id="bb1fe-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb1fe-123">Here is a JSON representation of the resource.</span></span>
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




