---
title: smsAuthenticationMethodTarget 资源类型
description: 已启用使用短信身份验证方法策略的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4309316adfeff126f845dd362d5ffb8899a77e60
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761028"
---
# <a name="smsauthenticationmethodtarget-resource-type"></a><span data-ttu-id="6b9c3-103">smsAuthenticationMethodTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b9c3-103">smsAuthenticationMethodTarget resource type</span></span>
<span data-ttu-id="6b9c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b9c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b9c3-105">在 Azure AD 中启用使用 [短信身份验证方法策略的用户](../resources/smsAuthenticationMethodConfiguration.md) 或组的集合。</span><span class="sxs-lookup"><span data-stu-id="6b9c3-105">A collection of users or groups enabled to use [Text Message authentication methods policy](../resources/smsAuthenticationMethodConfiguration.md) in Azure AD.</span></span>

## <a name="properties"></a><span data-ttu-id="6b9c3-106">属性</span><span class="sxs-lookup"><span data-stu-id="6b9c3-106">Properties</span></span>
|<span data-ttu-id="6b9c3-107">属性</span><span class="sxs-lookup"><span data-stu-id="6b9c3-107">Property</span></span>|<span data-ttu-id="6b9c3-108">类型</span><span class="sxs-lookup"><span data-stu-id="6b9c3-108">Type</span></span>|<span data-ttu-id="6b9c3-109">说明</span><span class="sxs-lookup"><span data-stu-id="6b9c3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b9c3-110">id</span><span class="sxs-lookup"><span data-stu-id="6b9c3-110">id</span></span>|<span data-ttu-id="6b9c3-111">String</span><span class="sxs-lookup"><span data-stu-id="6b9c3-111">String</span></span>|<span data-ttu-id="6b9c3-112">Azure AD 用户或组的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="6b9c3-112">Object ID of an Azure AD user or group.</span></span>|
|<span data-ttu-id="6b9c3-113">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="6b9c3-113">isRegistrationRequired</span></span>|<span data-ttu-id="6b9c3-114">布尔</span><span class="sxs-lookup"><span data-stu-id="6b9c3-114">Boolean</span></span>|<span data-ttu-id="6b9c3-115">确定是否强制用户注册身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="6b9c3-115">Determines whether the user is enforced to register the authentication method.</span></span> <span data-ttu-id="6b9c3-116">**不支持**。</span><span class="sxs-lookup"><span data-stu-id="6b9c3-116">**Not supported**.</span></span>|
|<span data-ttu-id="6b9c3-117">isUsableForSignIn</span><span class="sxs-lookup"><span data-stu-id="6b9c3-117">isUsableForSignIn</span></span>|<span data-ttu-id="6b9c3-118">布尔</span><span class="sxs-lookup"><span data-stu-id="6b9c3-118">Boolean</span></span>|<span data-ttu-id="6b9c3-119">确定用户或组能否使用此身份验证方法登录到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="6b9c3-119">Determines if the users or groups can use this authentication method to sign in to Azure AD.</span></span> <span data-ttu-id="6b9c3-120">该值始终为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="6b9c3-120">The value is always `true`.</span></span>|
|<span data-ttu-id="6b9c3-121">targetType</span><span class="sxs-lookup"><span data-stu-id="6b9c3-121">targetType</span></span>|<span data-ttu-id="6b9c3-122">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="6b9c3-122">authenticationMethodTargetType</span></span>| <span data-ttu-id="6b9c3-123">可取值为：`user`、`group`。</span><span class="sxs-lookup"><span data-stu-id="6b9c3-123">Possible values are: `user`, `group`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b9c3-124">关系</span><span class="sxs-lookup"><span data-stu-id="6b9c3-124">Relationships</span></span>
<span data-ttu-id="6b9c3-125">无。</span><span class="sxs-lookup"><span data-stu-id="6b9c3-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b9c3-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b9c3-126">JSON representation</span></span>
<span data-ttu-id="6b9c3-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b9c3-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.smsAuthenticationMethodTarget",
  "baseType": "microsoft.graph.authenticationMethodTarget",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethodTarget",
  "targetType": "String",
  "id": "String (identifier)",
  "isRegistrationRequired": "Boolean",
  "isUsableForSignIn": "Boolean"
}
```
