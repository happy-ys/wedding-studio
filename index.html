<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover" />
<title>웨딩 스튜디오 취향 셀렉트 · 내 취향 TOP 10</title>
<meta name="description" content="웨딩 스튜디오 65곳 중에서 1:1 비교로 내 취향 TOP 10을 뽑아보세요. 각 스튜디오 공식 포트폴리오 링크 포함." />
<meta property="og:title" content="웨딩 스튜디오 취향 셀렉트" />
<meta property="og:description" content="65곳 중에서 내 취향 TOP 10 뽑기 · 공식 포트폴리오 링크 포함" />
<meta property="og:type" content="website" />
<link rel="icon" href="data:image/svg+xml,%3Csvg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22%3E%3Ctext y=%22.9em%22 font-size=%2290%22%3E%F0%9F%92%8D%3C/text%3E%3C/svg%3E" />
<style>
  html,body{margin:0;padding:0}
  body{background:#F2EEEA;min-height:100vh;-webkit-text-size-adjust:100%}
  #root{min-height:100vh}
</style>
</head>
<body>
<div id="root"></div>
<script crossorigin src="https://unpkg.com/react@18/umd/react.production.min.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.production.min.js"></script>
<script>
const {
  useState,
  useMemo,
  useCallback,
  useEffect,
  useRef
} = React;

/* ───────────────────────── 데이터 ───────────────────────── */
const STUDIOS = ["21그램하우스", "S 스튜디오", "고유", "어바이드 (구.그사순)", "그레이스케일", "꼬모 스튜디오", "노우드", "느와르블랑하우스", "다다스튜디오 리허설", "라앤디", "라크마", "랑게", "로 스튜디오하우스", "로그에이", "르노브", "리저브하우스", "멜로필드 스튜디오", "멜린", "모닌 스튜디오", "무이", "바로오늘이그날", "박개인주의", "발렌", "보어하우스", "볼라르", "부겐빌리아", "비마이", "비비엔다", "비슈어", "세미앙", "세인트지지오티하우스", "소네", "소르아", "소피소", "스튜디오 콜레트", "스튜디오 피프티", "식스플로어", "아우드", "아이브", "아카이브", "아키", "아테소", "아트버스픽쳐", "앤드류권", "에버른", "오브라마에스트라", "오중석스튜디오", "원규", "유온드", "이경호 포토그라피 스튜디오", "이브로제", "일드한남", "제이유 스튜디오", "줄리의정원", "지엥마지", "카마스튜디오", "클로드", "테이크마인드", "포에버마인", "플라츠", "플레하우스", "피아", "헤이스", "헤이쥬드", "헤이허니"];

/* ───────────────── 머지소트 엔진 (사람 비교 기반) ───────────────── */
// runs: 정렬된 부분리스트들의 큐. merge: 진행 중인 병합 상태.
function normalize(engine) {
  let runs = engine.runs.slice();
  let merge = engine.merge;
  while (true) {
    if (merge) {
      if (merge.li >= merge.left.length || merge.ri >= merge.right.length) {
        const merged = merge.out.concat(merge.left.slice(merge.li)).concat(merge.right.slice(merge.ri));
        runs.push(merged);
        merge = null;
        continue;
      }
      return {
        runs,
        merge
      }; // 비교 필요
    } else {
      if (runs.length <= 1) return {
        runs,
        merge: null
      }; // 완료
      const left = runs.shift();
      const right = runs.shift();
      merge = {
        left,
        right,
        li: 0,
        ri: 0,
        out: []
      };
      continue;
    }
  }
}
function applyPick(engine, side) {
  const m = engine.merge;
  if (!m) return engine;
  const out = m.out.slice();
  let {
    li,
    ri
  } = m;
  if (side === "left") {
    out.push(m.left[li]);
    li += 1;
  } else {
    out.push(m.right[ri]);
    ri += 1;
  }
  return normalize({
    runs: engine.runs.slice(),
    merge: {
      ...m,
      li,
      ri,
      out
    }
  });
}
function initEngine(items) {
  return normalize({
    runs: items.map(x => [x]),
    merge: null
  });
}
function shuffle(arr) {
  const a = arr.slice();
  for (let i = a.length - 1; i > 0; i--) {
    const j = Math.floor(Math.random() * (i + 1));
    [a[i], a[j]] = [a[j], a[i]];
  }
  return a;
}

/* ───────────────────────── 스타일 ───────────────────────── */
const C = {
  bg: "#F2EEEA",
  card: "#FCFAF8",
  ink: "#26221F",
  taupe: "#8B8178",
  hair: "#E2DBD3",
  accent: "#7C4A52",
  accentSoft: "#EFE3E2"
};
const serif = "'Nanum Myeongjo','Noto Serif KR',Georgia,'Times New Roman',serif";
const sans = "-apple-system,BlinkMacSystemFont,'Apple SD Gothic Neo','Pretendard','Malgun Gothic',sans-serif";
const CSS = `
@import url('https://fonts.googleapis.com/css2?family=Nanum+Myeongjo:wght@400;700;800&display=swap');
.wsp-root *{box-sizing:border-box;margin:0;padding:0}
.wsp-root{font-family:${sans};color:${C.ink};background:${C.bg};
  min-height:560px;width:100%;display:flex;justify-content:center;
  padding:32px 18px 44px;-webkit-font-smoothing:antialiased}
.wsp-stage{width:100%;max-width:540px}
.wsp-fade{animation:wspFade .32s ease}
@keyframes wspFade{from{opacity:0;transform:translateY(6px)}to{opacity:1;transform:none}}
.wsp-eyebrow{font-size:11px;letter-spacing:.22em;text-transform:uppercase;
  color:${C.accent};font-weight:700}
.wsp-rule{height:1px;background:${C.hair};border:0}

.wsp-choice{width:100%;text-align:left;background:${C.card};cursor:pointer;
  border:1px solid ${C.hair};border-radius:14px;padding:22px 22px;
  font-family:${serif};font-size:24px;color:${C.ink};line-height:1.3;
  transition:transform .12s ease,border-color .15s ease,box-shadow .15s ease;
  position:relative;display:flex;align-items:center;min-height:96px}
.wsp-choice:hover{border-color:${C.accent};box-shadow:0 6px 22px rgba(38,34,31,.07)}
.wsp-choice:active{transform:scale(.985)}
.wsp-choice:focus-visible{outline:2px solid ${C.accent};outline-offset:3px}
.wsp-choice.flash{border-color:${C.accent};background:${C.accentSoft}}
.wsp-kbd{position:absolute;top:12px;right:14px;font-family:${sans};
  font-size:10px;letter-spacing:.06em;color:${C.taupe};border:1px solid ${C.hair};
  border-radius:6px;padding:2px 7px;background:${C.bg}}

.wsp-samples{display:flex;gap:8px;justify-content:center;margin-top:10px;flex-wrap:wrap}
.wsp-samples a{font-family:${sans};font-size:12px;letter-spacing:.02em;color:${C.taupe};
  text-decoration:none;border:1px solid ${C.hair};border-radius:999px;padding:6px 13px;
  background:${C.card};transition:all .14s ease;display:inline-flex;align-items:center;gap:5px}
.wsp-samples a:hover{color:${C.accent};border-color:${C.accent}}
.wsp-samples a:focus-visible{outline:2px solid ${C.accent};outline-offset:2px}
.wsp-samples a.wsp-primary{color:${C.accent};border-color:${C.accent};background:${C.accentSoft};font-weight:600}
.wsp-samples a.wsp-primary:hover{background:${C.accent};color:#fff}

.wsp-btn{font-family:${sans};cursor:pointer;border-radius:11px;
  padding:14px 18px;font-size:15px;font-weight:600;transition:all .14s ease;
  border:1px solid ${C.hair};background:${C.card};color:${C.ink}}
.wsp-btn:hover{border-color:${C.accent}}
.wsp-btn:active{transform:scale(.97)}
.wsp-btn:focus-visible{outline:2px solid ${C.accent};outline-offset:2px}
.wsp-btn.pass{color:${C.taupe}}
.wsp-btn.pass:hover{color:${C.ink}}
.wsp-btn.like{background:${C.ink};color:${C.bg};border-color:${C.ink}}
.wsp-btn.like:hover{background:${C.accent};border-color:${C.accent}}
.wsp-btn.primary{background:${C.accent};color:#fff;border-color:${C.accent};
  width:100%;padding:16px;font-size:16px}
.wsp-btn.primary:hover{filter:brightness(1.06)}
.wsp-btn.ghost{background:transparent;border-color:transparent;color:${C.taupe};
  font-size:13px;padding:8px 10px}
.wsp-btn.ghost:hover{color:${C.ink};border-color:transparent}
.wsp-btn:disabled{opacity:.35;cursor:not-allowed}

.wsp-progress{height:3px;background:${C.hair};border-radius:3px;overflow:hidden}
.wsp-progress>i{display:block;height:100%;background:${C.accent};
  border-radius:3px;transition:width .3s ease}

.wsp-rankrow{display:flex;align-items:baseline;gap:16px;padding:13px 0;
  border-bottom:1px solid ${C.hair}}
.wsp-num{font-family:${serif};font-size:20px;color:${C.accent};
  min-width:34px;font-weight:700;font-variant-numeric:tabular-nums}
.wsp-name{font-family:${serif};font-size:20px;line-height:1.25}

@media (max-width:430px){
  .wsp-choice{font-size:21px;min-height:88px;padding:20px}
  .wsp-name{font-size:18px}
}
@media (prefers-reduced-motion:reduce){
  .wsp-fade{animation:none}
  .wsp-choice,.wsp-btn,.wsp-progress>i{transition:none}
}
`;

/* ───────────────────────── 컴포넌트 ───────────────────────── */
/* ───────────── 공식 직링크 (홈페이지 우선, 없으면 공식 인스타) ───────────── */
const cleanName = n => n.replace(/\s*\(.*?\)\s*/g, " ").replace(/\s+/g, " ").trim();
const LINKS = {
  "21그램하우스": "https://www.instagram.com/21gram_official/",
  "S 스튜디오": "https://www.instagram.com/studios_company/",
  "고유": "https://www.instagram.com/studio.goyou/",
  "어바이드 (구.그사순)": "https://www.instagram.com/he_love_moment/",
  "그레이스케일": "https://gray-scale.co.kr/",
  "꼬모 스튜디오": "https://www.instagram.com/ccomostudio_official/",
  "노우드": "http://www.noud.kr/",
  "느와르블랑하우스": "http://www.noirblanc.co.kr/",
  "다다스튜디오 리허설": "https://www.instagram.com/dada.studio.roseselavy/",
  "라앤디": "https://www.instagram.com/laendy_studio/",
  "라크마": "https://www.instagram.com/lacmastudio/",
  "랑게": "https://www.instagram.com/langhe_official/",
  "로 스튜디오하우스": "https://ro-studio.co.kr/",
  "로그에이": "https://www.studiologa.com/",
  "르노브": "https://www.instagram.com/langhe_official/",
  "리저브하우스": "https://reservehaus.com/",
  "멜로필드 스튜디오": "https://www.instagram.com/melofield/",
  "멜린": "https://www.instagram.com/mellinstudio/",
  "모닌 스튜디오": "https://www.instagram.com/moninstudio/",
  "무이": "http://mui.co.kr/",
  "바로오늘이그날": "https://www.instagram.com/today_is_the_day_studio/",
  "박개인주의": "https://www.instagram.com/individual_ism/",
  "발렌": "https://valenestudio.com/",
  "보어하우스": "https://www.instagram.com/vohrhaus/",
  "볼라르": "https://www.instagram.com/studio__volare/",
  "부겐빌리아": "https://www.instagram.com/bougain.villea35/",
  "비마이": "https://www.instagram.com/_bemy_studio/",
  "비비엔다": "https://www.obrapictures.co.kr/VIVIENDA",
  "비슈어": "http://besure.co.kr/",
  "세미앙": "https://www.instagram.com/_semia.n/",
  "세인트지지오티하우스": "http://www.stggot.com/",
  "소네": "https://www.instagram.com/studiosonne/",
  "소르아": "https://www.sorrawedding.com/",
  "소피소": "https://soffiso.kr/",
  "스튜디오 콜레트": "https://www.instagram.com/studio___colette/",
  "스튜디오 피프티": "https://www.instagram.com/50.studio_fifty_/",
  "식스플로어": "https://www.instagram.com/st_sixth_floor/",
  "아우드": "https://www.instagram.com/aoud_studio/",
  "아이브": "https://www.instagram.com/studio__ive/",
  "아카이브": "http://archive-studio.com/",
  "아키": "https://www.instagram.com/arkki_studio/",
  "아테소": "https://www.instagram.com/ateso_official/",
  "아트버스픽쳐": "https://www.artbusterpicture.com/",
  "앤드류권": "https://www.andrewkwon.co.kr/",
  "에버른": "https://www.instagram.com/everne_studio/",
  "오브라마에스트라": "https://www.obrapictures.co.kr/",
  "오중석스튜디오": "https://geniusoh.kr/",
  "원규": "https://www.wonkyu.co.kr/",
  "유온드": "https://www.instagram.com/uond.photography/",
  "이경호 포토그라피 스튜디오": "https://www.leekyungho-photograph.com/",
  "이브로제": "https://www.instagram.com/yvesrose_haus/",
  "일드한남": "https://www.instagram.com/ile_de_hannam/",
  "제이유 스튜디오": "https://www.ju-photography.com/justudio",
  "줄리의정원": "http://www.juliesgarden.co.kr/",
  "지엥마지": "https://www.instagram.com/sienmarge_st/",
  "카마스튜디오": "https://www.kamastudio.co.kr/",
  "클로드": "https://www.instagram.com/studio__claude/",
  "테이크마인드": "https://www.instagram.com/takemind/",
  "포에버마인": "https://forevermine.co.kr/",
  "플라츠": "https://www.instagram.com/platz_people/",
  "플레하우스": "https://www.instagram.com/plaehouse/",
  "피아": "https://studiofia.com/",
  "헤이스": "https://www.instagram.com/studiohayes/",
  "헤이쥬드": "https://www.instagram.com/heyjude_st/",
  "헤이허니": "https://www.instagram.com/heyhoney_st/"
};
const naverUrl = name => `https://search.naver.com/search.naver?query=${encodeURIComponent(cleanName(name) + " 웨딩스튜디오")}`;
const linkLabel = url => url && url.includes("instagram.com") ? "인스타그램 ↗" : "홈페이지 ↗";
function SampleLinks({
  name
}) {
  const url = LINKS[name];
  return /*#__PURE__*/React.createElement("div", {
    className: "wsp-samples"
  }, url ? /*#__PURE__*/React.createElement("a", {
    className: "wsp-primary",
    href: url,
    target: "_blank",
    rel: "noopener noreferrer"
  }, "포트폴리오 · ", linkLabel(url)) : /*#__PURE__*/React.createElement("a", {
    className: "wsp-primary",
    href: `https://www.google.com/search?tbm=isch&q=${encodeURIComponent(cleanName(name) + " 웨딩")}`,
    target: "_blank",
    rel: "noopener noreferrer"
  }, "사진 검색 ↗"), /*#__PURE__*/React.createElement("a", {
    href: naverUrl(name),
    target: "_blank",
    rel: "noopener noreferrer"
  }, "네이버 ↗"));
}

/* ───────────────────────── 컴포넌트 ───────────────────────── */
function WeddingStudioPicker() {
  const [phase, setPhase] = useState("intro"); // intro | filter | rank | done
  // 필터
  const [idx, setIdx] = useState(0);
  const [liked, setLiked] = useState([]);
  const [filterHist, setFilterHist] = useState([]); // {idx, choice}
  // 랭킹
  const [engine, setEngine] = useState(null);
  const [rankHist, setRankHist] = useState([]);
  const [flash, setFlash] = useState(null); // 'left'|'right'
  const [copied, setCopied] = useState(false);
  const [showAll, setShowAll] = useState(false);
  const lockRef = useRef(false);

  /* ---------- 필터 단계 ---------- */
  const filterDecide = useCallback(like => {
    setFilterHist(h => [...h, {
      idx,
      choice: like
    }]);
    if (like) setLiked(l => [...l, STUDIOS[idx]]);
    if (idx + 1 >= STUDIOS.length) startRank(like ? [...liked, STUDIOS[idx]] : liked);else setIdx(i => i + 1);
  }, [idx, liked] // eslint-disable-line
  );
  const filterUndo = useCallback(() => {
    setFilterHist(h => {
      if (!h.length) return h;
      const last = h[h.length - 1];
      if (last.choice) setLiked(l => l.slice(0, -1));
      setIdx(last.idx);
      return h.slice(0, -1);
    });
  }, []);
  const startRank = useCallback(pool => {
    const items = shuffle(pool);
    setEngine(initEngine(items));
    setRankHist([]);
    setPhase(items.length <= 1 ? "done" : "rank");
    if (items.length <= 1) finalizeFrom(items.length === 1 ? initEngine(items) : null, items);
  }, []); // eslint-disable-line

  const finalizeFrom = () => {}; // placeholder (완료 판정은 렌더에서)

  /* ---------- 랭킹 단계 ---------- */
  const pick = useCallback(side => {
    if (!engine || !engine.merge || lockRef.current) return;
    lockRef.current = true;
    setFlash(side);
    setTimeout(() => {
      setRankHist(h => [...h, engine]);
      setEngine(e => applyPick(e, side));
      setFlash(null);
      lockRef.current = false;
    }, 130);
  }, [engine]);
  const rankUndo = useCallback(() => {
    setRankHist(h => {
      if (!h.length) return h;
      setEngine(h[h.length - 1]);
      return h.slice(0, -1);
    });
  }, []);
  const isDone = engine && !engine.merge && engine.runs.length <= 1;
  const result = isDone ? engine.runs[0] || [] : [];
  useEffect(() => {
    if (phase === "rank" && isDone) setPhase("done");
  }, [phase, isDone]);

  /* ---------- 키보드 ---------- */
  useEffect(() => {
    const h = e => {
      if (phase === "filter") {
        if (e.key === "ArrowLeft") {
          e.preventDefault();
          filterDecide(false);
        }
        if (e.key === "ArrowRight") {
          e.preventDefault();
          filterDecide(true);
        }
        if ((e.key === "Backspace" || e.key === "z") && filterHist.length) {
          e.preventDefault();
          filterUndo();
        }
      } else if (phase === "rank" && engine?.merge) {
        if (e.key === "ArrowUp" || e.key === "1") {
          e.preventDefault();
          pick("left");
        }
        if (e.key === "ArrowDown" || e.key === "2") {
          e.preventDefault();
          pick("right");
        }
        if ((e.key === "Backspace" || e.key === "z") && rankHist.length) {
          e.preventDefault();
          rankUndo();
        }
      }
    };
    window.addEventListener("keydown", h);
    return () => window.removeEventListener("keydown", h);
  }, [phase, engine, filterDecide, filterUndo, pick, rankUndo, filterHist.length, rankHist.length]);

  /* ---------- 진행률 ---------- */
  const estTotal = useMemo(() => {
    const n = liked.length || 1;
    return Math.max(1, Math.ceil(n * Math.log2(Math.max(2, n))));
  }, [liked.length]);
  const comparisons = rankHist.length;
  const rankPct = isDone ? 100 : Math.min(99, Math.round(comparisons / estTotal * 100));
  const restart = () => {
    setPhase("intro");
    setIdx(0);
    setLiked([]);
    setFilterHist([]);
    setEngine(null);
    setRankHist([]);
    setFlash(null);
    setCopied(false);
    setShowAll(false);
  };
  const reRank = () => {
    setEngine(initEngine(shuffle(liked)));
    setRankHist([]);
    setCopied(false);
    setShowAll(false);
    setPhase("rank");
  };
  const copyTop = () => {
    const top = result.slice(0, 10);
    const text = "내 웨딩 스튜디오 취향 TOP " + top.length + "\n" + top.map((s, i) => `${i + 1}. ${s}`).join("\n");
    navigator.clipboard?.writeText(text).then(() => {
      setCopied(true);
      setTimeout(() => setCopied(false), 1800);
    }, () => {});
  };

  /* ───────────────────────── 렌더 ───────────────────────── */
  return /*#__PURE__*/React.createElement("div", {
    className: "wsp-root"
  }, /*#__PURE__*/React.createElement("style", null, CSS), /*#__PURE__*/React.createElement("div", {
    className: "wsp-stage"
  }, phase === "intro" && /*#__PURE__*/React.createElement("div", {
    className: "wsp-fade"
  }, /*#__PURE__*/React.createElement("p", {
    className: "wsp-eyebrow"
  }, "웨딩 스튜디오 취향 셀렉트"), /*#__PURE__*/React.createElement("h1", {
    style: {
      fontFamily: serif,
      fontSize: 34,
      lineHeight: 1.22,
      margin: "14px 0 18px",
      fontWeight: 800
    }
  }, "65곳 중에서", /*#__PURE__*/React.createElement("br", null), "내 취향 TOP 10을 찾아요"), /*#__PURE__*/React.createElement("hr", {
    className: "wsp-rule"
  }), /*#__PURE__*/React.createElement("ol", {
    style: {
      listStyle: "none",
      margin: "22px 0 26px"
    }
  }, /*#__PURE__*/React.createElement("li", {
    style: {
      display: "flex",
      gap: 14,
      marginBottom: 18
    }
  }, /*#__PURE__*/React.createElement("span", {
    style: {
      fontFamily: serif,
      color: C.accent,
      fontSize: 18,
      fontWeight: 700
    }
  }, "01"), /*#__PURE__*/React.createElement("span", {
    style: {
      fontSize: 15,
      lineHeight: 1.55,
      color: C.ink
    }
  }, /*#__PURE__*/React.createElement("b", {
    style: {
      fontWeight: 700
    }
  }, "빠르게 추리기"), " — 한 곳씩 보며 끌리면 좋아요, 아니면 패스. 각 카드의 ", /*#__PURE__*/React.createElement("b", {
    style: {
      fontWeight: 700
    }
  }, "포트폴리오"), " 링크로 그 스튜디오의 공식 홈페이지·인스타를 바로 열어볼 수 있어요.")), /*#__PURE__*/React.createElement("li", {
    style: {
      display: "flex",
      gap: 14
    }
  }, /*#__PURE__*/React.createElement("span", {
    style: {
      fontFamily: serif,
      color: C.accent,
      fontSize: 18,
      fontWeight: 700
    }
  }, "02"), /*#__PURE__*/React.createElement("span", {
    style: {
      fontSize: 15,
      lineHeight: 1.55,
      color: C.ink
    }
  }, /*#__PURE__*/React.createElement("b", {
    style: {
      fontWeight: 700
    }
  }, "1:1로 순위 매기기"), " — 남은 곳끼리 둘씩 비교. 진 곳도 제대로 줄세워서 상위 10개가 흔들리지 않아요."))), /*#__PURE__*/React.createElement("button", {
    className: "wsp-btn primary",
    onClick: () => setPhase("filter")
  }, "시작하기"), /*#__PURE__*/React.createElement("p", {
    style: {
      fontSize: 12.5,
      color: C.taupe,
      marginTop: 14,
      lineHeight: 1.5
    }
  }, "단판 이상형월드컵은 1등엔 좋지만 2등부터 순위가 엉켜요. 이 방식은 전체를 비교해 정렬하기 때문에 “상위 10개”에 더 정확합니다.")), phase === "filter" && /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      justifyContent: "space-between",
      alignItems: "center",
      marginBottom: 10
    }
  }, /*#__PURE__*/React.createElement("span", {
    className: "wsp-eyebrow"
  }, "STEP 01 · 추리기"), /*#__PURE__*/React.createElement("span", {
    style: {
      fontSize: 13,
      color: C.taupe,
      fontVariantNumeric: "tabular-nums"
    }
  }, idx + 1, " / ", STUDIOS.length, " · 찜 ", liked.length)), /*#__PURE__*/React.createElement("div", {
    className: "wsp-progress",
    style: {
      marginBottom: 26
    }
  }, /*#__PURE__*/React.createElement("i", {
    style: {
      width: `${idx / STUDIOS.length * 100}%`
    }
  })), /*#__PURE__*/React.createElement("div", {
    className: "wsp-choice wsp-fade",
    key: idx,
    style: {
      justifyContent: "center",
      minHeight: 150,
      fontSize: 30,
      textAlign: "center"
    }
  }, STUDIOS[idx]), /*#__PURE__*/React.createElement(SampleLinks, {
    name: STUDIOS[idx]
  }), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "grid",
      gridTemplateColumns: "1fr 1fr",
      gap: 12,
      marginTop: 18
    }
  }, /*#__PURE__*/React.createElement("button", {
    className: "wsp-btn pass",
    onClick: () => filterDecide(false)
  }, "패스 ", /*#__PURE__*/React.createElement("span", {
    style: {
      opacity: .5,
      fontSize: 12
    }
  }, "←")), /*#__PURE__*/React.createElement("button", {
    className: "wsp-btn like",
    onClick: () => filterDecide(true)
  }, /*#__PURE__*/React.createElement("span", {
    style: {
      opacity: .6,
      fontSize: 12
    }
  }, "→"), " 좋아요")), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      justifyContent: "space-between",
      alignItems: "center",
      marginTop: 18
    }
  }, /*#__PURE__*/React.createElement("button", {
    className: "wsp-btn ghost",
    onClick: filterUndo,
    disabled: !filterHist.length
  }, "← 되돌리기"), /*#__PURE__*/React.createElement("button", {
    className: "wsp-btn ghost",
    style: {
      color: liked.length >= 2 ? C.accent : C.taupe
    },
    onClick: () => startRank(liked),
    disabled: liked.length < 2
  }, "그만 보고 순위 매기기 →")), /*#__PURE__*/React.createElement("p", {
    style: {
      fontSize: 12,
      color: C.taupe,
      marginTop: 16,
      textAlign: "center",
      lineHeight: 1.5
    }
  }, "10개 이상 찜해두면 TOP 10이 깔끔하게 나와요.")), phase === "rank" && engine?.merge && /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      justifyContent: "space-between",
      alignItems: "center",
      marginBottom: 10
    }
  }, /*#__PURE__*/React.createElement("span", {
    className: "wsp-eyebrow"
  }, "STEP 02 · 1:1 대결"), /*#__PURE__*/React.createElement("span", {
    style: {
      fontSize: 13,
      color: C.taupe,
      fontVariantNumeric: "tabular-nums"
    }
  }, "비교 ", comparisons, "회")), /*#__PURE__*/React.createElement("div", {
    className: "wsp-progress",
    style: {
      marginBottom: 8
    }
  }, /*#__PURE__*/React.createElement("i", {
    style: {
      width: `${rankPct}%`
    }
  })), /*#__PURE__*/React.createElement("p", {
    style: {
      fontSize: 13,
      color: C.taupe,
      textAlign: "center",
      margin: "14px 0 18px"
    }
  }, "더 끌리는 곳은?"), /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("button", {
    className: "wsp-choice" + (flash === "left" ? " flash" : ""),
    onClick: () => pick("left"),
    style: {
      justifyContent: "center",
      textAlign: "center",
      width: "100%"
    }
  }, /*#__PURE__*/React.createElement("span", {
    className: "wsp-kbd"
  }, "↑ 또는 1"), engine.merge.left[engine.merge.li]), /*#__PURE__*/React.createElement(SampleLinks, {
    name: engine.merge.left[engine.merge.li]
  })), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "flex",
      alignItems: "center",
      gap: 14,
      margin: "16px 2px"
    }
  }, /*#__PURE__*/React.createElement("span", {
    style: {
      flex: 1,
      height: 1,
      background: C.hair
    }
  }), /*#__PURE__*/React.createElement("span", {
    style: {
      fontFamily: serif,
      fontStyle: "italic",
      color: C.taupe,
      fontSize: 15,
      letterSpacing: ".05em"
    }
  }, "vs"), /*#__PURE__*/React.createElement("span", {
    style: {
      flex: 1,
      height: 1,
      background: C.hair
    }
  })), /*#__PURE__*/React.createElement("div", null, /*#__PURE__*/React.createElement("button", {
    className: "wsp-choice" + (flash === "right" ? " flash" : ""),
    onClick: () => pick("right"),
    style: {
      justifyContent: "center",
      textAlign: "center",
      width: "100%"
    }
  }, /*#__PURE__*/React.createElement("span", {
    className: "wsp-kbd"
  }, "↓ 또는 2"), engine.merge.right[engine.merge.ri]), /*#__PURE__*/React.createElement(SampleLinks, {
    name: engine.merge.right[engine.merge.ri]
  })), /*#__PURE__*/React.createElement("div", {
    style: {
      textAlign: "center",
      marginTop: 20
    }
  }, /*#__PURE__*/React.createElement("button", {
    className: "wsp-btn ghost",
    onClick: rankUndo,
    disabled: !rankHist.length
  }, "← 방금 선택 되돌리기"))), phase === "done" && /*#__PURE__*/React.createElement("div", {
    className: "wsp-fade"
  }, /*#__PURE__*/React.createElement("p", {
    className: "wsp-eyebrow"
  }, "취향 셀렉트 완성"), /*#__PURE__*/React.createElement("h2", {
    style: {
      fontFamily: serif,
      fontSize: 30,
      margin: "12px 0 6px",
      fontWeight: 800
    }
  }, "내 웨딩 스튜디오 TOP ", Math.min(10, result.length)), /*#__PURE__*/React.createElement("p", {
    style: {
      fontSize: 13,
      color: C.taupe,
      marginBottom: 22
    }
  }, liked.length, "곳을 추려 ", comparisons, "번의 비교로 줄세웠어요."), result.slice(0, 10).map((s, i) => /*#__PURE__*/React.createElement("div", {
    className: "wsp-rankrow wsp-fade",
    key: s,
    style: {
      animationDelay: `${i * 0.04}s`
    }
  }, /*#__PURE__*/React.createElement("span", {
    className: "wsp-num"
  }, String(i + 1).padStart(2, "0")), /*#__PURE__*/React.createElement("span", {
    className: "wsp-name",
    style: {
      flex: 1
    }
  }, s), /*#__PURE__*/React.createElement("a", {
    href: LINKS[s] || naverUrl(s),
    target: "_blank",
    rel: "noopener noreferrer",
    style: {
      fontFamily: sans,
      fontSize: 12,
      color: C.accent,
      textDecoration: "none",
      whiteSpace: "nowrap"
    }
  }, "포트폴리오 ↗"))), result.length < 10 && /*#__PURE__*/React.createElement("p", {
    style: {
      fontSize: 13,
      color: C.taupe,
      marginTop: 14,
      lineHeight: 1.5
    }
  }, "찜한 곳이 ", result.length, "곳이라 TOP 10을 다 채우진 못했어요. 더 뽑으려면 처음부터 다시 시작해 좋아요를 늘려보세요."), result.length > 10 && /*#__PURE__*/React.createElement("div", {
    style: {
      marginTop: 20
    }
  }, /*#__PURE__*/React.createElement("button", {
    className: "wsp-btn ghost",
    style: {
      color: C.accent
    },
    onClick: () => setShowAll(v => !v)
  }, showAll ? "전체 순위 접기 ▲" : `11위~${result.length}위 전체 보기 ▼`), showAll && /*#__PURE__*/React.createElement("div", {
    style: {
      marginTop: 8
    }
  }, result.slice(10).map((s, i) => /*#__PURE__*/React.createElement("div", {
    className: "wsp-rankrow",
    key: s
  }, /*#__PURE__*/React.createElement("span", {
    className: "wsp-num",
    style: {
      color: C.taupe,
      fontSize: 16
    }
  }, i + 11), /*#__PURE__*/React.createElement("span", {
    className: "wsp-name",
    style: {
      fontSize: 17,
      color: C.taupe
    }
  }, s))))), /*#__PURE__*/React.createElement("div", {
    style: {
      display: "grid",
      gridTemplateColumns: "1fr 1fr",
      gap: 12,
      marginTop: 28
    }
  }, /*#__PURE__*/React.createElement("button", {
    className: "wsp-btn",
    onClick: copyTop
  }, copied ? "복사됨 ✓" : "TOP 10 복사"), /*#__PURE__*/React.createElement("button", {
    className: "wsp-btn",
    onClick: reRank,
    disabled: liked.length < 2
  }, "같은 후보 다시 정렬")), /*#__PURE__*/React.createElement("button", {
    className: "wsp-btn ghost",
    style: {
      width: "100%",
      marginTop: 10
    },
    onClick: restart
  }, "처음부터 다시"))));
}
ReactDOM.createRoot(document.getElementById("root")).render(/*#__PURE__*/React.createElement(WeddingStudioPicker, null));
</script>
</body>
</html>
