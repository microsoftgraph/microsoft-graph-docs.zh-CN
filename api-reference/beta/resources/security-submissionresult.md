---
title: submissionResult 资源类型
description: 表示 Microsoft 处理威胁提交后的评审结果。
author: caigen
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 302a37636fa66fae386e660c34d59f72f1ca2e0f
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856688"
---
# <a name="submissionresult-resource-type"></a>submissionResult 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 Microsoft 处理威胁提交后的评审结果。

## <a name="properties"></a>属性
| 属性           | 类型                               | Description                                                             |
|:-------------------|:-----------------------------------|:------------------------------------------------------------------------|
| category           | submissionResultCategory           | 提交结果类别。 可能的值是：`notJunk`、、`spam`、`malware``phishing`、`allowedByPolicy`、`blockedByPolicy``spoof`、`unknown``noResultAvailable`和 。`unkownFutureValue` |
| 详细             | [security.submissionResultDetail](#submissionresultdetail-values)             | 指定 Microsoft 提供的其他详细信息，以证实其分析结果。 |
| detectedFiles      | collection ([security.submissionDetectedFile](../resources/security-submissiondetectedfile.md))  | 指定 Microsoft 在提交的电子邮件中检测到的文件。|
| detectedUrls       | 集合（字符串）                 | 指定 Microsoft 在提交的电子邮件中检测到的 URL。|
| userMailboxSetting | [security.userMailboxSetting](#usermailboxsetting-values) | 指定由逗号分隔字符串表示的用户邮箱设置。 |

### <a name="usermailboxsetting-values"></a>userMailboxSetting 值
| 成员  | 说明 |
| :----------------- | :------------------------------------ |
| 无 | 没有与此威胁提交相关的用户邮箱设置。 |
| junkMailDeletion | 提交的电子邮件应用了垃圾邮件删除。 |
| isFromAddressInAddressBook | 提交的电子邮件来自通讯簿中的地址。 |
| isFromAddressInAddressSafeList | 提交的电子邮件来自地址安全列表中的地址。 |
| isFromAddressInAddressBlockList | 提交的电子邮件来自地址安全列表中的地址。 |
| isFromAddressInAddressImplicitSafeList | 提交的电子邮件来自地址隐式安全列表中的地址。 |
| isFromAddressInAddressImplicitJunkList | 提交的电子邮件来自地址隐式垃圾邮件列表中的地址。 |
| isFromDomainInDomainSafeList | 提交的电子邮件来自域安全列表中的域。 |
| isFromDomainInDomainBlockList | 提交的电子邮件来自域块列表中的域。 |
| isRecipientInRecipientSafeList | 提交的电子邮件是收件人安全列表中的收件人。 |
| customRule | 提交的电子邮件由一个用户自定义规则处理。 |
| senderPraPresent | 提交的电子邮件来自之前提供过的发件人。 |
| fromFirstTimeSender | 提交的电子邮件来自第一次发件人。 |
| 独家 | 提交的电子邮件的收件人是收件人的通讯簿独有的，而仅允许通讯簿联系人发送。 |
| priorSeenPass | 之前看到已提交的电子邮件已通过。 |
| senderAuthenticationSucceeded | 已提交电子邮件的发件人身份验证已成功。 |
| isJunkMailRuleEnabled | 已启用垃圾邮件规则。 |
| unknownFutureValue | 未知的未来值。 |

### <a name="submissionresultdetail-values"></a>submissionResultDetail 值
| 成员                                  | 说明                                                  |
| :------------------------------------- | :----------------------------------------------------------- |
| 无                                   | Microsoft 没有有关要共享的结果的其他详细信息。            |
| underInvestigation                     | Microsoft 仍在分析示例，结果应很快可用。      |
| simulatedThreat                        |  报告的消息被阻止，因为它是发送给用户进行网络钓鱼教育的网络钓鱼模拟电子邮件。 配置 EOP/MDO 以允许其签出高级交付|
| allowedBySecOps                          | 报告的消息是由于安全操作员邮箱的高级传递流而允许的。 因此，将其从高级交付中删除以阻止它 |
| allowedByThirdPartyFilters             | 报告的消息是允许/阻止的，因为第三方筛选器与 EOP/MDO 协同工作。 配置增强的筛选，以便 EOP/MDO 能够准确筛选   |
| messageNotFound                        | Microsoft 无法对报告的消息做出判决，因为 Microsoft 找不到实际消息。 请在 security.microsoft.com 中使用提交上传电子邮件重新提交 |
| urlFileShouldNotBeBlocked              | Microsoft 发现报告的实体是干净的。 包含它的现有电子邮件已发布。 网络钓鱼和恶意软件筛选器将在几周后从中学习。 在此之前，若要允许，请在租户允许/阻止列表中创建允许条目（如果尚未完成）。 |
| urlFileShouldBeBlocked                 | Microsoft 发现报告的实体是恶意的。 包含该电子邮件的现有电子邮件已被隔离。 网络钓鱼和恶意软件筛选器将在几周后从中学习。 在此之前，若要阻止它，请在租户允许/阻止列表中创建块条目（如果尚未完成） |
| urlFileCannotMakeDecision              | Microsoft 目前无法做出判决。 重新提交，以便在分析后对其作出判决。 如果尚未完成，请使用租户允许/阻止列表立即允许/阻止它。 |
| domainImpersonation                    | 由于域模拟策略设置，报告的消息被允许/阻止。 配置域模拟策略，以便 EOP/MDO 可以相应地筛选 |
| userImpersonation                      | 由于用户模拟策略设置，报告的消息被允许/阻止。 配置用户模拟策略，以便 EOP/MDO 可以相应地筛选 |
| brandImpersonation                     | 由于品牌模拟策略设置，报告的消息被允许/阻止。 配置品牌模拟策略，以便 EOP/MDO 可以相应地进行筛选 |
| outboundShouldNotBeBlocked             | 报告的传出消息已发现干净，Microsoft 将在未来几周内更新其基于机器学习的出站筛选器。 |
| outboundShouldBeBlocked                | 报告的传出消息被发现是恶意的，Microsoft 将在未来几周内更新其基于机器学习的出站筛选器。 |
| outboundBulk                           | Microsoft 发现报告的消息是垃圾邮件/垃圾邮件。 几周后将了解出站筛选器 |
| outboundCannotMakeDecision             | Microsoft 目前无法做出判决。 重新提交，以便在分析后对其做出判决。  |
| outboundNotRescanned                   | Microsoft 无法对报告的出站消息做出判决，因为 Microsoft 找不到实际消息。 请在 security.microsoft.com 中使用提交上传电子邮件重新提交 |
| zeroHourAutoPurgeAllowed               | 报告的消息被打碎，因为组织有零小时自动清除。 |
| zeroHourAutoPurgeBlocked               | 由于组织已关闭零小时自动清除，因此无法对报告的消息进行清理。 为 EOP/MDO 启用零小时自动清除，以便在消息在传递后变成恶意消息|
| zeroHourAutoPurgeQuarantineReleased    | 报告的消息已从隔离区释放，尽管由于 zap 而被隔离，因为消息在传递后变成恶意消息。 |
| onPremisesSkip                         | 报告的消息无法分析，因为这经过了 Exchange Online Protection 的本地设置。 配置混合安装程序，以便 EOP/MDO 可以在传送之前扫描邮件以交换本地邮箱 |
| allowedByTenantAllowBlockList          | 报告的消息是允许的，因为电子邮件中的一个或多个实体位于租户允许/阻止列表中。 从租户允许/阻止列表中删除允许，以便 EOP/MDO 可以相应地筛选 |
| blockedByTenantAllowBlockList          | 报告的消息被阻止，因为电子邮件中的一个或多个实体位于租户允许/阻止列表中。 从租户允许/阻止列表中删除块，以便 EOP/MDO 可以相应地筛选 |
| allowedUrlByTenantAllowBlockList       | 已允许报告的 URL，因为它是在租户允许/阻止列表中。 从租户允许/阻止列表中删除允许，以便 EOP/MDO 可以相应地筛选 |
| allowedFileByTenantAllowBlockList      | 报告的文件是允许的，因为它是在租户允许/阻止列表中。 从租户允许/阻止列表中删除允许，以便 EOP/MDO 可以相应地筛选 |
| allowedSenderByTenantAllowBlockList    | 报告的消息是允许的，因为电子邮件的发件人位于租户允许/阻止列表中。 从租户允许/阻止列表中删除允许，以便 EOP/MDO 可以相应地筛选|
| allowedRecipientByTenantAllowBlockList | 报告的传出消息是允许的，因为收件人位于租户允许/阻止列表中。 从租户允许/阻止中删除允许，以便 EOP/MDO 可以相应地筛选 |
| blockedUrlByTenantAllowBlockList       | 报告的 URL 被阻止，因为它位于租户允许/阻止列表中。 从租户允许/阻止列表中删除块，以便 EOP/MDO 可以相应地筛选 |
| blockedFileByTenantAllowBlockList      | 报告的文件被阻止，因为它位于租户允许/阻止列表中。 从租户允许/阻止列表中删除块，以便 EOP/MDO 可以相应地筛选 |
| blockedSenderByTenantAllowBlockList    | 报告的消息被阻止，因为电子邮件的发件人位于租户允许/阻止列表中。 从租户允许/阻止列表中删除块，以便 EOP/MDO 可以相应地筛选|
| blockedRecipientByTenantAllowBlockList | 报告的传出消息被阻止，因为收件人位于租户允许/阻止列表中。 从租户中删除块允许/阻止，以便 EOP/MDO 可以相应地筛选 |
| allowedByConnection                    | 报告的消息是允许的，因为发送 IP 位于托管连接筛选器策略上。 从托管连接筛选器策略中删除 IP，以便 EOP/MDO 可以相应地筛选 |
| blockedByConnection                    | 报告的消息被阻止，因为发送 IP 位于托管连接筛选器策略上。 从托管连接筛选器策略中删除 IP，以便 EOP/MDO 可以相应地筛选 |
| allowedByExchangeTransportRule         | 报告的消息是允许的，因为组织有相关的交换传输规则。 删除交换传输规则，以便 EOP/MDO 可以相应地进行筛选。 |
| blockedByExchangeTransportRule         | 报告的消息被阻止，因为组织有相关的交换传输规则。 删除交换传输规则，以便 EOP/MDO 可以相应地进行筛选。 |
| quarantineReleased                     | 报告的消息已从隔离区释放，尽管被 EOP/MDO 隔离 |
| quarantineReleasedThenBlocked          | 从隔离区释放后，报告的消息被用户设置阻止。 删除用户设置，以便将邮件发布到收件箱 |
| junkMailRuleDisabled                   | 报告的消息肯定会传递到垃圾文件夹，但垃圾文件夹已被禁用。 打开垃圾文件夹设置，以便 EOP/MDO 可以相应地传送电子邮件 |
| allowedByUserSetting                   | 由于 Outlook 中的用户安全或受信任的发件人设置，因此允许报告的消息。 删除安全或受信任的发件人设置，以便 EOP/MDO 可以相应地筛选 |
| blockedByUserSetting                   | 由于 outlook 中的用户阻止或受信任的发件人设置，报告的消息被阻止。 删除受阻止或受信任的发件人设置，以便 EOP/MDO 可以相应地进行筛选 |
| allowedByTenant                        | 由于租户策略或策略操作设置，允许报告的消息。 查看 EOP/MDO 策略或策略操作设置，以便 EOP/MDO 可以相应地进行筛选 |
| blockedByTenant                        | 由于租户策略或策略操作设置，报告的消息被阻止。 查看 EOP/MDO 策略或策略操作设置，以便 EOP/MDO 可以相应地进行筛选 |
| invalidFalsePositive                   | EOP/MDO 已允许报告的消息。                  |
| invalidFalseNegative                   | 报告的消息已被 EOP/MDO 阻止。                     |
| spoofBlocked                           | 报告的消息已由系统欺骗确定，因此被阻止。 在租户允许/阻止列表中创建欺骗允许，以便 EOP/MDO 可以允许来自此欺骗发件人的电子邮件    |
| goodReclassifiedAsBad                  | Microsoft 发现报告的消息是恶意的。 现有电子邮件已被隔离。 网络钓鱼和恶意软件筛选器将在几周后从中学习。 在此之前，若要阻止它，请在租户允许/阻止列表中创建块条目（如果尚未完成） |
| goodReclassifiedAsBulk                 | Microsoft 发现报告的消息是垃圾邮件。 几周后，垃圾邮件和批量筛选器将从中学习。 在此之前，若要阻止它，请在租户允许/阻止列表中创建块条目（如果尚未完成） |
| goodReclassifiedAsGood                 | Microsoft 发现报告的消息是干净的。 如果你不同意此判决，请重新提交电子邮件。 在此之前，若要阻止它，请在租户允许/阻止列表中创建块条目（如果尚未完成） |
| goodReclassifiedAsCannotMakeDecision   | Microsoft 目前无法做出判决。 重新提交，以便在分析后对其作出判决。 如果尚未完成，请使用租户允许/阻止列表立即阻止它。 |
| badReclassifiedAsGood                  | Microsoft 发现报告的消息是干净的。 现有电子邮件已发布。 网络钓鱼和恶意软件筛选器将在几周后从中学习。 在此之前，若要允许，请在租户允许/阻止列表中创建允许条目（如果尚未完成） |
| badReclassifiedAsBulk                  | Microsoft 发现报告的消息是垃圾邮件。 几周后，垃圾邮件和批量筛选器将从中学习。 在此之前，若要允许，请在租户允许/阻止列表中创建允许条目（如果尚未完成） |
| badReclassifiedAsBad                   | Microsoft 发现报告的消息是恶意的。 如果你不同意此判决，请重新提交电子邮件。 在此之前，若要允许，请在租户允许/阻止列表中创建允许条目（如果尚未完成） |
| badReclassifiedAsCannotMakeDecision    | Microsoft 目前无法做出判决。 重新提交，以便在分析后对其作出判决。 如果尚未完成，请使用租户允许/阻止列表立即允许它。 |
| unknownFutureValue                     | 任何将来未使用的值。                     |


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.submissionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.submissionResult",
  "category": "String",
  "detail": "String",
  "userMailboxSetting": "String",
  "detectedUrls": [
    "String"
  ],
  "detectedFiles": [
    {
      "@odata.type": "microsoft.graph.security.submissionDetectedFile"
    }
  ]
}
```

