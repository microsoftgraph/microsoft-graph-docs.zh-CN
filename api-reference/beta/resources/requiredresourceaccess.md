---
title: requiredResourceAccess 资源类型
description: 指定一组的 OAuth 2.0 权限范围和指定的资源的应用程序需要访问下的应用程序角色。 指定的 OAuth 2.0 权限范围可能请求 （通过**requiredResourceAccess**集合） 的客户端应用程序时调用资源应用程序。 应用程序实体的**requiredResourceAccess**属性是**ReqiredResourceAccess**的集合。
localization_priority: Normal
ms.openlocfilehash: a2c7e337bbe441275f395c2333b8cee918e6b9da
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512967"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="147ba-105">requiredResourceAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="147ba-105">requiredResourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="147ba-106">指定一组的 OAuth 2.0 权限范围和指定的资源的应用程序需要访问下的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="147ba-106">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="147ba-107">指定的 OAuth 2.0 权限范围可能请求 （通过**requiredResourceAccess**集合） 的客户端应用程序时调用资源应用程序。</span><span class="sxs-lookup"><span data-stu-id="147ba-107">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="147ba-108">[应用程序](application.md)实体的**requiredResourceAccess**属性是**ReqiredResourceAccess**的集合。</span><span class="sxs-lookup"><span data-stu-id="147ba-108">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="147ba-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="147ba-109">JSON representation</span></span>

<span data-ttu-id="147ba-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="147ba-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a><span data-ttu-id="147ba-111">属性</span><span class="sxs-lookup"><span data-stu-id="147ba-111">Properties</span></span>
| <span data-ttu-id="147ba-112">属性</span><span class="sxs-lookup"><span data-stu-id="147ba-112">Property</span></span>     | <span data-ttu-id="147ba-113">类型</span><span class="sxs-lookup"><span data-stu-id="147ba-113">Type</span></span>   |<span data-ttu-id="147ba-114">说明</span><span class="sxs-lookup"><span data-stu-id="147ba-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="147ba-115">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="147ba-115">resourceAccess</span></span>|<span data-ttu-id="147ba-116">[ResourceAccess](resourceaccess.md)集合</span><span class="sxs-lookup"><span data-stu-id="147ba-116">[ResourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="147ba-117">OAuth2.0 权限范围和应用程序需要从指定的资源的应用程序角色的列表。</span><span class="sxs-lookup"><span data-stu-id="147ba-117">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="147ba-118">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="147ba-118">resourceAppId</span></span>|<span data-ttu-id="147ba-119">String</span><span class="sxs-lookup"><span data-stu-id="147ba-119">String</span></span>|<span data-ttu-id="147ba-120">应用程序需要访问资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="147ba-120">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="147ba-121">这应该是等于**appId**上的目标资源应用程序声明。</span><span class="sxs-lookup"><span data-stu-id="147ba-121">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/requiredresourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
