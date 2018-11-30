---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
ms.openlocfilehash: 886ed1912c9c6626a06f1efaef83de5ed1f52a66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007610"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="b76db-103">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="b76db-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="b76db-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b76db-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b76db-105">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="b76db-105">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="b76db-106">属性</span><span class="sxs-lookup"><span data-stu-id="b76db-106">Properties</span></span>
|<span data-ttu-id="b76db-107">属性</span><span class="sxs-lookup"><span data-stu-id="b76db-107">Property</span></span>|<span data-ttu-id="b76db-108">类型</span><span class="sxs-lookup"><span data-stu-id="b76db-108">Type</span></span>|<span data-ttu-id="b76db-109">说明</span><span class="sxs-lookup"><span data-stu-id="b76db-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b76db-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="b76db-110">encryptionMethod</span></span>|[<span data-ttu-id="b76db-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="b76db-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="b76db-112">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="b76db-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="b76db-113">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="b76db-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="b76db-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="b76db-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="b76db-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="b76db-115">Boolean</span></span>|<span data-ttu-id="b76db-116">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="b76db-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="b76db-117">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="b76db-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="b76db-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="b76db-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="b76db-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b76db-119">Boolean</span></span>|<span data-ttu-id="b76db-120">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="b76db-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b76db-121">关系</span><span class="sxs-lookup"><span data-stu-id="b76db-121">Relationships</span></span>
<span data-ttu-id="b76db-122">无</span><span class="sxs-lookup"><span data-stu-id="b76db-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b76db-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b76db-123">JSON Representation</span></span>
<span data-ttu-id="b76db-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b76db-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```



