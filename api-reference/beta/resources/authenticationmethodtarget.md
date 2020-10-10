---
title: authenticationMethodTarget 资源类型
description: 在身份验证方法策略中启用使用身份验证方法的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7112249f618bbda31eddeb07967d201c8b641075
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418266"
---
# <a name="authenticationmethodtarget-resource-type"></a><span data-ttu-id="8472f-103">authenticationMethodTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="8472f-103">authenticationMethodTarget resource type</span></span>

<span data-ttu-id="8472f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8472f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8472f-105">启用身份验证方法的用户或组的集合，作为 Azure AD 中的身份验证方法策略的一部分。</span><span class="sxs-lookup"><span data-stu-id="8472f-105">A collection of users or groups enabled to use an authentication method as part of an authentication method policy in Azure AD.</span></span>


## <a name="properties"></a><span data-ttu-id="8472f-106">属性</span><span class="sxs-lookup"><span data-stu-id="8472f-106">Properties</span></span>
|<span data-ttu-id="8472f-107">属性</span><span class="sxs-lookup"><span data-stu-id="8472f-107">Property</span></span>|<span data-ttu-id="8472f-108">类型</span><span class="sxs-lookup"><span data-stu-id="8472f-108">Type</span></span>|<span data-ttu-id="8472f-109">说明</span><span class="sxs-lookup"><span data-stu-id="8472f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8472f-110">id</span><span class="sxs-lookup"><span data-stu-id="8472f-110">id</span></span>|<span data-ttu-id="8472f-111">字符串</span><span class="sxs-lookup"><span data-stu-id="8472f-111">String</span></span>|<span data-ttu-id="8472f-112">Azure AD 用户或组的对象 Id。</span><span class="sxs-lookup"><span data-stu-id="8472f-112">Object Id of an Azure AD user or group.</span></span>|
|<span data-ttu-id="8472f-113">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="8472f-113">isRegistrationRequired</span></span>|<span data-ttu-id="8472f-114">布尔</span><span class="sxs-lookup"><span data-stu-id="8472f-114">Boolean</span></span>|<span data-ttu-id="8472f-115">确定是否强制用户注册身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="8472f-115">Determines if the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="8472f-116">targetType</span><span class="sxs-lookup"><span data-stu-id="8472f-116">targetType</span></span>|<span data-ttu-id="8472f-117">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="8472f-117">authenticationMethodTargetType</span></span>|<span data-ttu-id="8472f-118">可取值为：`user`、`group`。</span><span class="sxs-lookup"><span data-stu-id="8472f-118">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="8472f-119">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="8472f-119">useForSignIn</span></span>|<span data-ttu-id="8472f-120">布尔</span><span class="sxs-lookup"><span data-stu-id="8472f-120">Boolean</span></span>|<span data-ttu-id="8472f-121">确定身份验证方法是否可用于登录 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="8472f-121">Determines if the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8472f-122">关系</span><span class="sxs-lookup"><span data-stu-id="8472f-122">Relationships</span></span>
<span data-ttu-id="8472f-123">无。</span><span class="sxs-lookup"><span data-stu-id="8472f-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8472f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8472f-124">JSON representation</span></span>
<span data-ttu-id="8472f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8472f-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodTarget",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean"
}
```
