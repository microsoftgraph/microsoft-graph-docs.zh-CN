---
title: certificateAuthority 资源类型
description: 表示证书颁发机构。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 50555ff47d81d96def360fe55fe8684f6ff07994
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531948"
---
# <a name="certificateauthority-resource-type"></a><span data-ttu-id="e58bf-103">certificateAuthority 资源类型</span><span class="sxs-lookup"><span data-stu-id="e58bf-103">certificateAuthority resource type</span></span>

<span data-ttu-id="e58bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e58bf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e58bf-105">表示证书颁发机构。</span><span class="sxs-lookup"><span data-stu-id="e58bf-105">Represents a certificate authority.</span></span>

## <a name="properties"></a><span data-ttu-id="e58bf-106">属性</span><span class="sxs-lookup"><span data-stu-id="e58bf-106">Properties</span></span>

| <span data-ttu-id="e58bf-107">属性</span><span class="sxs-lookup"><span data-stu-id="e58bf-107">Property</span></span>     | <span data-ttu-id="e58bf-108">类型</span><span class="sxs-lookup"><span data-stu-id="e58bf-108">Type</span></span>        | <span data-ttu-id="e58bf-109">说明</span><span class="sxs-lookup"><span data-stu-id="e58bf-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e58bf-110">证书</span><span class="sxs-lookup"><span data-stu-id="e58bf-110">certificate</span></span>|<span data-ttu-id="e58bf-111">Binary</span><span class="sxs-lookup"><span data-stu-id="e58bf-111">Binary</span></span>|<span data-ttu-id="e58bf-112">必需。</span><span class="sxs-lookup"><span data-stu-id="e58bf-112">Required.</span></span> <span data-ttu-id="e58bf-113">表示公共证书的 base64 编码字符串。</span><span class="sxs-lookup"><span data-stu-id="e58bf-113">The base64 encoded string representing the public certificate.</span></span>|
|<span data-ttu-id="e58bf-114">certificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="e58bf-114">certificateRevocationListUrl</span></span>|<span data-ttu-id="e58bf-115">字符串</span><span class="sxs-lookup"><span data-stu-id="e58bf-115">String</span></span>|<span data-ttu-id="e58bf-116">证书吊销列表的 URL。</span><span class="sxs-lookup"><span data-stu-id="e58bf-116">The URL of the certificate revocation list.</span></span>|
|<span data-ttu-id="e58bf-117">deltaCertificateRevocationListUrl</span><span class="sxs-lookup"><span data-stu-id="e58bf-117">deltaCertificateRevocationListUrl</span></span>|<span data-ttu-id="e58bf-118">字符串</span><span class="sxs-lookup"><span data-stu-id="e58bf-118">String</span></span>|<span data-ttu-id="e58bf-119">该 URL 包含自上次创建完整证书 revocaton 列表以来的所有已吊销证书的列表。</span><span class="sxs-lookup"><span data-stu-id="e58bf-119">The URL contains the list of all revoked certificates since the last time a full certificate revocaton list was created.</span></span>|
|<span data-ttu-id="e58bf-120">isRootAuthority</span><span class="sxs-lookup"><span data-stu-id="e58bf-120">isRootAuthority</span></span>|<span data-ttu-id="e58bf-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="e58bf-121">Boolean</span></span>|<span data-ttu-id="e58bf-122">必需。</span><span class="sxs-lookup"><span data-stu-id="e58bf-122">Required.</span></span> <span data-ttu-id="e58bf-123">如果受信任的证书是根证书颁发机构，**则为 true** ; 如果受信任的证书是中间颁发机构，则为**false** 。</span><span class="sxs-lookup"><span data-stu-id="e58bf-123">**true** if the trusted certificate is a root authority, **false** if the trusted certificate is an intermediate authority.</span></span>|
|<span data-ttu-id="e58bf-124">常用</span><span class="sxs-lookup"><span data-stu-id="e58bf-124">issuer</span></span>|<span data-ttu-id="e58bf-125">字符串</span><span class="sxs-lookup"><span data-stu-id="e58bf-125">String</span></span>|<span data-ttu-id="e58bf-126">证书的颁发者，根据**证书**值计算。</span><span class="sxs-lookup"><span data-stu-id="e58bf-126">The issuer of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="e58bf-127">只读。</span><span class="sxs-lookup"><span data-stu-id="e58bf-127">Read-only.</span></span> |
|<span data-ttu-id="e58bf-128">issuerSki</span><span class="sxs-lookup"><span data-stu-id="e58bf-128">issuerSki</span></span>|<span data-ttu-id="e58bf-129">字符串</span><span class="sxs-lookup"><span data-stu-id="e58bf-129">String</span></span>|<span data-ttu-id="e58bf-130">证书的主题密钥标识符，由**证书**值计算得出。</span><span class="sxs-lookup"><span data-stu-id="e58bf-130">The subject key identifier of the certificate, calculated from the **certificate** value.</span></span> <span data-ttu-id="e58bf-131">只读。</span><span class="sxs-lookup"><span data-stu-id="e58bf-131">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e58bf-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e58bf-132">JSON representation</span></span>

<span data-ttu-id="e58bf-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e58bf-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateAuthority",
  "baseType": null
}-->

```json
{
  "certificate": "Binary",
  "certificateRevocationListUrl": "String",
  "deltaCertificateRevocationListUrl": "String",
  "isRootAuthority": true,
  "issuer": "String",
  "issuerSki": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateAuthority resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->